# ansible-airflow

## Пререквизиты
На локальной машине должен быть установлен ansible:

`sudo apt install ansible`

## Описание
В данном проекте в качестве удаленной машины используется `localhost`. Удаленные хосты можно настроить в `inventory` файле.

`playbook` содержит в себе две роли: `docker` и `airflow` для установки и настройки соответствующих сервисов. 

Для более детальной конфигурации `airflow` используется файл `airflow.cfg` в директории `/roles/airflow/files/airflow.cfg`.


## Запускаем проект
`sudo ansible-playbook -i inventory playbook.yaml`