# ansible-airflow

## Пререквизиты
На локальной машине должен быть установлен ansible:

`sudo apt install ansible`

## Описание
В данном проекте в качестве удаленной машины используется `localhost`. Удаленные хосты можно настроить в `inventory` файле.

`Playbook` содержит в себе две роли: `docker` и `airflow` для установки и настройки соответствующих сервисов. 

Для более детальной конфигурации `airflow` используется файл `airflow.cfg` в директории `/roles/airflow/files/airflow.cfg`.

Airflow webserver будет доступен по адресу `localhost:8080`

## Запускаем проект
`sudo ansible-playbook -i inventory playbook.yaml`

