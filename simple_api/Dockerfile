FROM python:3.11-slim
LABEL maintainer="Liedji-kouedjeu-Emmanuel"
RUN apt update -y && apt install python-dev-is-python3 python3-dev libsasl2-dev libldap2-dev libssl-dev build-essential -y
COPY student_age.py /student_age.py
COPY requirements.txt /requirements.txt
RUN pip3 install -r /requirements.txt
RUN mkdir /data
VOLUME /data
EXPOSE 5000
CMD ["python3", "./student_age.py"]
