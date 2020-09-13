FROM ubuntu:latest


RUN groupadd -r airflow && useradd -r -g airflow airflow
RUN apt-get update -y

RUN apt-get install -y \
    python3.6 \
    python3-pip


ENV AIRFLOW_HOME /opt/airflow 
RUN mkdir /opt/airflow && pip3 install psycopg2-binary && pip3 install apache-airflow[aws,kubernetes,postgres] 
RUN chown -R airflow /opt/airflow
USER airflow
CMD echo "helloworld"