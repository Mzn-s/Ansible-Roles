# Install Jenkins Server on Centos 7
Данная Ansible роль выполняет развёртывание Jenkins сервера на удалённом хосте.
Используемой операционной системой является Centos 7.
В конце установки всех необходимых пакетов, ansible возвращает Login-code Jenkins, необходимый для первичной авторизации на сервере.

Порядок выполняемых действий:
1. Установка пакета OpenJDK 8.
2. Установка Wget.
3. Подключение Jenkins репозитория.
4. Импорт ключа Jenkins.
5. Установка Jenkins.
6. Открытие порта 8080 в firewall.
7. Рестарт firewall.
8. Запуск service Jenkins.
9. Ожидание появления файла AdminPassword.
10. Отображение содержимого данного файла.

# Install Webserver with Webpage Centos & Ubuntu
Эта роль Ansible устанавивает веб-сервер Apache операционные системы Cenos 7 и на Ubuntu OS и отображает тестовый Website.

Порядок выполняемых действий:
1. Проверка и вывод семейства ОС, на которую планируется установка сервера.
2. Установка и запуск Apache на RedHat или Debian.
3. Открытие порта 80/tcp в firewall.
4. Копирование файлов на удалённый хост.

Так же данная роль имеет handlers, с проверкой статуса Apache и его перезапуском, при необходимости.
