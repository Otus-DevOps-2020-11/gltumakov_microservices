# docker-2 HMW
## Что сделано?
– настроен travis и pre-commit для работы с новым репозиторием;
– с помощью команды `docker commit <container_id>` создан образ запущенного контейнера;
– вывод команды `docker images`, содержащий данные о созданном образе, записан в файл "/dockermonolith/docker-1.log";
– выполнено задание со "\*": на основе анализа различий в выводе команды `docker inspect` для образа и контейнера, объяснение добавлено в файл "dockermonolith/docker-1.log");
– выполненa установка docker-machine (больше не идет в пакете с Docker Desktop для MacOS);
– создан Docker host в Yandex Cloud;
– через `docker-machine create ...; eval $(docker-machine env docker-host)` локальное окружение настроено для работы с удаленным хостом;
– в директории "dockermonolith/" создан Dockerfile и др. файлы, указанные в ДЗ;
– выполнены команды build и run для запуска контейнера на удаленном хосте;
– для загрузки нашего образа в Docker Hub выполнены команды: docker login, docker build, docker tag, docker push;
– локально запущен контейнер, созданный из образа, загруженного в Docker Hub
