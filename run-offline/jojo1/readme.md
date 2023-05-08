#комментарии по развертыванию сервера для таска Отсылка на ДжоДжо 1 у себя:

Если к вас не установлен docker, установите: [https://selectel.ru/blog/docker-install-ubuntu/](на linux); [https://learn.microsoft.com/ru-ru/virtualization/windowscontainers/manage-docker/configure-docker-daemon](на windows)
Распакуйте jojo1.zip в отдельную папку, откройте в ней терминал и напишите:
```
docker build . -t jojo_reference
docker run -p 8002:8000 -d --name jojo_reference jojo_reference
```
Дальше, скачайте main.html, распакуйте архив images.zip туда же и откройте main.html.