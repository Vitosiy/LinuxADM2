## Jenkins

0) Развернули на второй машине nginx:
![](images/6.png)

1) Запулил образ jenkins в систему:
![](images/1.png)

2) Запуск докер-контейнера:
![](images/2.png)

3) Делаю листинг для проверки и достаю пароль:
![](images/3.png)

4) Вошли и делаем установку:

![](images/4.png)

![](images/5.png)

5) Welcome to Jenkins!:
![](images/7.png)

6) Создаем freestyle project:
![](images/8.png)

7) Создал репозиторий на GitHub, откуда будем тянуть изменения:
![](images/15.jpg)

8) Сделал базовые изменения в index.html:
![](images/16.jpg)

9) Ставим плагин для SSH:
![](images/9.png)

10) Настраиваем SSH и проверяем соединение:
![](images/10.png)

11) Собираем проект:
![](images/11.png)

12) Страница nginx:
![](images/12.png)

13) Вносим изменения в репозитории и пушим:
![](images/17.jpg)

14) Изменения задеплоились минуту спустя:
![](images/13.png)

----

## Gitlab

1) Написал docker-compose.yml с gitlab и gitlab-runner для ci\cd:

![](images/18.png)

2) Поднимаем docker-compose:

![](images/19.png)

3) Листинг контейнеров:

![](images/20.png)

4) Достаем пароль рута для входа на GitLab:

![](images/21.png)

5) Вошли:

![](images/22.png)

5) Регистрируем gitlab-runner:

![](images/23.png)

6) Создаем проект и пишем в нем .gitlab-ci.yml:

![](images/24.png)

7) Создаем переменную $SSH_PASS со значением 1:

![](images/25.png)

8) Собралось и задеплоилось: 

![](images/26.png)

![](images/28.jpg)

9) Страница nginx после деплоя:

![](images/27.png)
