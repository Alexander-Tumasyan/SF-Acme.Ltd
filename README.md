# SF-Acme.Ltd

Main repository

## Расположение репозитория с кодом

Ссылка на проект - <https://github.com/Alexander-Tumasyan/test.git>

Для просмотра проекта можно воспользоваться IDE Visual Studio Code - <https://code.visualstudio.com/>

Скачать проект к себе на локальный компьютер:

git clone git@github.com:Alexander-Tumasyan/SF-Acme.Ltd.git - Предварительно должен быть создан/добавлен ключ SSH

Инструкция по установке - <https://docs.github.com/ru/authentication/connecting-to-github-with-ssh/about-ssh>

git clone <https://github.com/Alexander-Tumasyan/SF-Acme.Ltd.git>

## Процесс внесения своих изменений в основную кодовую базу и правила наименования веток

Основная ветка проекта main. В неё вливаются изменения через Pull request. Новые ветки разработки создаются только от main-ветки. Ветвления типа «main-ветка-ветка» запрещены. Каждая новая ветка разработки должна быть привязана к задаче в Trello, то есть имя должно быть идентично имени задачи. Пример feature-task1, где task1 – наименование задачи. Для наглядности данная ветка добавлена в проект.

Инструкция по использованию Pull request - <https://docs.github.com/ru/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request>

## Среда разработки и файл конфигурации

Устанавливаем Git - <https://git-scm.com/>
После установки можно воспользоваться файлом конфига, который находится в проекте. Заменить в блоке [user] значения email и name на свои. Так же для упрощения просмотра логов добавлена команда git history.

Команды, которые дополняют конфиг:

git config --global user.name "имя"

git config --global user.email "адрес почтового ящика"

git config --global alias.history 'log --graph'

## Инструкция для младших сотрудников по слиянию веток, какие команды надо выполнить, чтобы

### создать свою ветку

git branch имя_ветки, потом надо перейти в ветку при помощи команды git checkout имя_ветки

git checkout -b имя_ветки - создание и переход на ветку

### внести изменения в нее

git add . или git add имя_файла

Затем git commit или git commit -m "", в ковычках указываем комментарий для коммита

### слить эти изменения с основной кодовой базой

Изменения в main вносятся через pull request. Описаны команды для понимания процесса слияния своих локальных веток.
Если надо в ветку main влить ветку feature-task1. Для начала надо переключиться на ту ветку, в которую будем вливать, а затем уже мержить.

git checkout main

git merge feature-task1
