# Логика работы playbook
Выполняется установка необходимых пакетов в зависимости от ОС (реализованы самые популярные) будут использован соответствующие менеджеры пакетов. Далее создаются необходимые файлы (скрипт phpinfo и файл виртуального хоста для веб-сервера), выполняется проверка синтаксиса nginx. В случае возникновения ошибок - ansible сообщит об ошибке характерным сообщением, если ошибки отсутствуют - будет произведено отключение дефолтного сайта nginx и активация новой конфигурации, а так же будет произведена перезагрузка веб-сервера и добавление его в автозагрузку при старте ОС.

# Запуск playbooks
Запуск playbooks выполняется командой ansible-playbook, например: ansible-playbook nginx_congigure.yml

![] (https://tadviser.ru/images/7/7a/Logo-Ansible-%D0%94%D1%8E%D1%80%D1%85%D0%B5%D0%BC.png)

![] (C:\Users\HP\Desktop\Netology\ansible_for_avito\Logo-Ansible-Дюрхем.png)