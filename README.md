# Git. Different commands

[1] Удалить комиты до нужного комита:
* git reset --hard commitId && git clean -f
* git push -f
* Узнать commitId можно из команды: git log --oneline
* Источник: https://stackoverflow.com/questions/4114095/how-do-i-revert-a-git-repository-to-a-previous-commit
  
[2] Создать проект в IDEA с исключением SonarLint из Git можно так::
* создаем проект в IDEA, без инициализации git
* в .gitignore добавил:\
.idea/sonarlint/\
.idea/sonarlint/**
* выполняем БЕЗ "sudo" следующие команды:
* cd ...путь к проекту
* git init
* git config --global --add safe.directory '/home/stalker/Документы/LearnJava-Prj/BlackBelt13'
* git add .
* git config --global user.email "mazurovyura09@yandex.ru"
* git commit -m "начало"
* (добавление на сайт)
* git remote add origin https://github.com/Yura-0910/BlackBelt.git
* git branch -M coreBranch13
* git push -uf origin coreBranch13
* (см. файл:: /home/stalker/Документы/LearnJava-Prj/Git-BlackBelt13-FOR-SONARLINTER)
