## Домашнее задание к занятию 7 «Жизненный цикл ПО»

## Шкутов Иван Владимирович

### Подготовка к выполнению

Получить бесплатную версию Jira - https://www.atlassian.com/ru/software/jira/work-management/free (скопируйте ссылку в адресную строку). Вы можете воспользоваться любым(в том числе бесплатным vpn сервисом) если сайт у вас недоступен. Кроме того вы можете скачать docker образ и запустить на своем хосте self-managed версию jira.

Настроить её для своей команды разработки.

Создать доски Kanban и Scrum.

Дополнительные инструкции от разработчика Jira.

### Основная часть

Необходимо создать собственные workflow для двух типов задач: bug и остальные типы задач. Задачи типа bug должны проходить жизненный цикл:

    Open -> On reproduce.
    On reproduce -> Open, Done reproduce.
    Done reproduce -> On fix.
    On fix -> On reproduce, Done fix.
    Done fix -> On test.
    On test -> On fix, Done.
    Done -> Closed, Open.
    Остальные задачи должны проходить по упрощённому workflow:

    Open -> On develop.
    On develop -> Open, Done develop.
    Done develop -> On test.
    On test -> On develop, Done.
    Done -> Closed, Open.
    
Что нужно сделать

1. Создайте задачу с типом bug, попытайтесь провести его по всему workflow до Done.

2. Создайте задачу с типом epic, к ней привяжите несколько задач с типом task, проведите их по всему workflow до Done.

3. При проведении обеих задач по статусам используйте kanban.

4. Верните задачи в статус Open.

5. Перейдите в Scrum, запланируйте новый спринт, состоящий из задач эпика и одного бага, стартуйте спринт, проведите задачи до состояния Closed. Закройте спринт.

6. Если всё отработалось в рамках ожидания — выгрузите схемы workflow для импорта в XML. Файлы с workflow и скриншоты workflow приложите к решению задания.

### Как оформить решение задания

Выполненное домашнее задание пришлите в виде ссылки на .md-файл в вашем репозитории.

![1](https://github.com/Ivan-Shkutov/ci-01-intro/blob/main/1.png)

![2](https://github.com/Ivan-Shkutov/ci-01-intro/blob/main/2.png)

![3](https://github.com/Ivan-Shkutov/ci-01-intro/blob/main/3.png)

![4](https://github.com/Ivan-Shkutov/ci-01-intro/blob/main/4.png)

![5](https://github.com/Ivan-Shkutov/ci-01-intro/blob/main/5.png)

![6](https://github.com/Ivan-Shkutov/ci-01-intro/blob/main/6.png)

![7](https://github.com/Ivan-Shkutov/ci-01-intro/blob/main/7.png)
