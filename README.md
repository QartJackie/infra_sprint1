# KITTYGRAM
Социальная сеть для любителей семейства кошачьих.

Стек:

 - Python 3.2
 - Django REST 
 - Simple JWT
 - Sentry-SDK
 - Gunicorn 20.1.0
 
Tree - утилита просмотра дерева директории:

    sudo apt install tree

Обновление списка доступных пакетов в Ubuntu:

    sudo apt update

Установка пакетов Python:

    sudo apt install python3-pip python3-venv -y

Создать виртуальное окружение:

    sudo apt-get python3 -m venv venv


Установить зависимости:

    pip install -r requirements.txt

Активировать окружение:

    source vevn/bin/activate/
Применить миграции:

    python manage.py migrate

Создать суперпользователя:

    python manage.py createsuperuser
Установить пакетный менеджер для React - npm:

    curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash - &&\
    sudo apt-get install -y nodejs
Версия npm:

    npm -v
 
Собрать статику:


Установить gunicorn:

    pip install gunicorn==20.1.0

Запуск gunicorn:

    gunicorn --bind 0.0.0.0:8000 backend.wsgi

Создание юнита для автозапуска gunicorn:

    sudo nano /etc/systemd/system/gunicorn.service

Запуск демона:

    старт демона:
    sudo systemctl start gunicorn 

	добавить автозапуск:
    sudo systemctl enable gunicorn
    
    статус:
    sudo systemctl status gunicorn

Установить nginx:

    sudo apt install nginx -y
Запустить сервер nginx:

    sudo systemctl start nginx

Включитьь фаервол для шифрования:

    sudo ufw allow 'Nginx Full'
    sudo ufw allow OpenSSH
    sudo ufw enable
    sudo ufw status


Файл конфигурации nginx:

    sudo nano /etc/nginx/sites-enabled/default

Проверка конфигурации nginx:

    nginx -t
  
Собрать статику:

    React app:
    npm run build

    Django app:
	python3 manage.py collectstatic

Скопировать статику:

    sudo cp -r kittygram/backend/static_backend/ /var/www/kittygram


