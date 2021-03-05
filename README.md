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
```
git branch newbranch1
git branch newbranch2
git branch
Видем:
* main
  newbr1
  newbr2
```
##
Bнести изменения в ветку 1 и 2
Переключимся на ветку
git chechout newbranch1
git status
echo "new text for newbranch1" > fileferst.txt
git add *
git commit
git status
Работа со второй веткой
git checkout newbranch2
echo "new text for newbranch2" > filesecond.txt
git status
git add *
git commit
Посмотрим, что получилось:
git log -n 2 --graph --all
root@homework6git:/home/mikekey/mikedevops/Homework6# git log -n 2 --graph --all
* commit 768a64a9b5b3eb9b90102380ee72ddfa1cbc6915 (HEAD -> newbranch2)
| Author: mixxod <mixxod@mail.com>
| Date:   Fri Mar 5 09:02:49 2021 +0000
|
|     new branch2 and new description
|
| * commit 930cb7abb3fa9fde78125b699f338a9167bf5902 (newbranch1)
|/  Author: mixxod <mixxod@mail.com>
|   Date:   Fri Mar 5 09:00:09 2021 +0000
|
|       add new branck and new description
```


  164  git merge newbranch1 -m "merge newbranch1 >newbranch2"
  165  git log -n 2 --graph --all
  166  git checkout main
  167  git branch
  168  git merge newbranch2 -m "merge newbranch2 >main"
  169  git log -n 2 --graph --all
  170  git reset --hard HEAD~1
  171  git log -n 2 --graph --all
  172  git push
  173  git status
  174  git branch
  175  git add *
  176  git commit
  177  git checkout newbranch1
  178  git add *
  179  git commit
  180  ls
  181  git status
  182  git push --set-upstream original main
  183  git push --set-upstream origin main
  184  git status
  185  git chechout main
  186  git check\out main
  187  git status
  188  git branch
  189  git branch -d develop
  190  git branch
  191  git add *
  192  git commit
  193  git push
  194  git branch
  195  git branch -r
  196  git branch --help
  197  git push -u origin newbrach1
  198  git push -u origin newbranch1
  199  git push -u origin newbranch2
  200  git branch
  201  git push origin --delete develop

