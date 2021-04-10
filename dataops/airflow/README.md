# impacta
Docker Composer utilizado para criação do Apache Airflow Localmente para uso de laboratório.


## Pré Requisitos
- Sistema Operacional Linux ou MacOs
- git               - https://git-scm.com/downloads
- docker            - https://docs.docker.com/get-docker/
- docker compose    - https://docs.docker.com/compose/install/

## Setup
```
git clone https://github.com/danilosousadba/impacta.git
```
### Criar os diretórios baixo e dar a permissão. Esses diretórios serão utilizados pelos containers do Airflow
```
mkdir -p /opt/airflow/dags
mkdir -p /opt/airflow/logs
mkdir -p /opt/airflow/plugins
chmod -R 775 /opt/airflow/
```
```
mkdir -p /opt/airflow/dags /opt/airflow/logs /opt/airflow/plugins
```
```
cd dataops/airflow
```
```
docker-compose up -d
```
## Default url
http://localhost:8080

## Default Username
airflow

## Default Password
airflow
