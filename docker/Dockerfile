FROM ubuntu:latest

RUN apt-get update -y

RUN apt-get install -y \
    python3.6 \
    python3-pip


ENV AIRFLOW_HOME /opt/airflow
RUN pip3 install psycopg2-binary && pip3 install apache-airflow[aws,kubernetes,postgres] 

CMD echo "helloworld"