### README

Данный playbook устанавливает на целевую машину нижеперечисленные сервисы:

- clickhouse_role
- lighthouse_role
- vector_role

Предварительно необходимо скачать роли, которые описаны в файле requirements.yml с помощью команды: ansible-galaxy role install -r requirements.yml -p ./roles

Затем запустить playbook с помощью команды: ansible-playbook -i inventory/prod.yaml site.yaml -vv