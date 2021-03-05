# Homework6
Homework6_GIT
Задачи:
1. Создать отдельный репозиторий на github.
2. Создать локально три текстовых файла.
3. Поместить в стейдж, закомитить, запушить.
4. Создать две новые ветки.
5. Внести изменения в ветку 1 и 2 
6. Смерджить между собой вновь созданные ветки.
7. Смерджить ветку с веткой мастер
8. Отменить предыдущий комит
9. Все изменения запушить в гит репозиторий.

=======================================================
##
```
Практическая часть:
1.Необходимо представиться ГИТу(делается один раз):
git config --global user.name "mixxod"
git config --global user.email "mixxod@gmail.com"
Создаем рабочий каталог
mkdir mikedevops
Инициализируем GIT
git init
Видем (mc), что пояилась скрытый каталог /.git
Создадим несколько файлов 
root@homework6git:/home/mikekey/mikedevops# echo "first test file" > first.test
root@homework6git:/home/mikekey/mikedevops# echo "second test file" > second.test
root@homework6git:/home/mikekey/mikedevops# echo "therd test file" > therd.test
Проверяем git status
Добавляем git add *
Коммитрим git commit или можно так: git commit -m "My files"
Делаем клон подготовленного репозитория c github
git clone https://github.com/mixxod/Homework6.git
переносим созданные файлы в каталог склонированного репозитория
git push


```
##
Создание веток и работа с ними

