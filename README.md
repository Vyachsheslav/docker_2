Из корневой директории последовательно выполняем команды:

создаем образ приложения
docker build -t my_app_crud -f ./docker/app/Dockerfile .

запускаем контейнер
docker run --name=my_app -d -p 8080:8000 my_app_crud

ссылка на приложение
http://localhost:8080/api/v1/