# What is this?

This contains the code to create the docker containers for the Webserver, the Scheduler and the Worker nodes for Airflow.

The airflow-web path contains the code to generate a python 3.x(latest on Ubuntu 16.04) image of an airflow webserver.

The airflow-sched path contains the code to generate a python 3.x(latest on Ubuntu 16.04) image of an airflow scheduler.

The airflow-wrkr path contains the code to generate a python 3.x(latest on Ubuntu 16.04) image of an airflow worker.

The airflow images also have the following additions / assumptions:

- AIRFLOW_HOME is /usr/local/airflow
- Task logs will be sent to S3 bucket using settings in Airflow config
- Airflow service logs are located in the cloudwatch logs for the task

Currently supported version of Airflow: 1.10.1
