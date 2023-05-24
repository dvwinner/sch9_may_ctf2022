# комментарии по развертыванию сервера для калькулятор у себя:

Если к вас не установлен docker, установите: [на linux](https://selectel.ru/blog/docker-install-ubuntu/); [на windows](https://learn.microsoft.com/ru-ru/virtualization/windowscontainers/manage-docker/configure-docker-daemon)

Распакуйте calculator.zip в отдельную папку, откройте в ней терминал и напишите:
```
docker build . -t jojo_reference
docker run -p 8002:8000 -d --name jojo_reference jojo_reference
```
Дальше, скачайте main.html в ту же папку и откройте main.html.