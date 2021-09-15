Что делает playbook install kibana:
1. С помощью модуля get_url скачивает программу kibana и копирует в указанную папку 

2. С помощью модуля file cоздает директорию kibana_home
(kibana_home: "/opt/kibana/{{ kibana_version }}")

3. С помощью модуля unarchive разархивирует скаченный архив и кладет его в нужную папку 

4. Прописываем программу kibana в переменное окружение 

Tags: kibana

hosts: ansible1 - это виртуальная машина поднятая на yandex cloud 
Playbook выполняется без ошибок (все оишбики какие были исправил)
 
ansible1: ok=13   changed=0    unreachable=0    failed=0    skipped=3    rescued=0    ignored=0


Из папки Files пришлось удалить файл jdk-11.0.12_linux-x64_bin.tar.gz, так как github стоит огранисение в 100mb 
