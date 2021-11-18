## mysql replication

1) Поднимаем gitlab + runner из прошлой лабы:

[docker-compose.yml](docker-compose.yml)

2) Регистрируем runner как в прошлой лабе, executor - shell

3) Создаем проект для репликации, в CI пишем наш скрипт:

[.gitlab-ci.yml](.gitlab-ci.yml)

4) Сам docker-compose для mysql:

[docker-compose-mysql.yml](docker-compose-mysql.yml)

Кладём его в проект на Gitlab

5) Запускаем pipeline

![1.png](images/1.png)

![2.png](images/2.png)

![3.png](images/3.png)

![4.png](images/4.png)

![5.png](images/5.png)

![6.png](images/6.png)

![7.png](images/7.png)

![8.png](images/8.png)
