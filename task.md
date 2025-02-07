# Инструкция по работе с git репозиторием

## Для начала работы:
> git init

Если имя пользователя и почта не были заданы:

> git config --user.name

> git config --user.email 

## Работа с файлами:

Для того чтобы добавить файл нужно:

1. >git add file_name
    добавляем файл с именем file_name для отслеживания
2. >git commit -m"some message"

* добавляем текущие изменения в репозиторий и подписываем их с помощью тега -m
* если добавить тег -а, то к комиту добавяться все измененные файлы, которые уже отслеживались

## Чтобы отслеживать состояние репозитория:

1. >git status
2. >git log

   Чтобы показать ветки:
   >git log --graph

3. >git diff

## Работа с коммитами

Для того чтобы перейти к определенному коммиту можно использовать команду:

> git checkout code_commit 
> code_commit-код коммита к которому хотим перейти, его можно посмотреть в git log

Чтобы вернуться к самому последнему состоянию:

> git checkout master

## Оформление внешнего вида

1. Для создания заголовка в начале строки пишем # или ##
2. Для выделения текста курсивом обрамите его звездочками*:

 *курсив*
    
3. Для выделения текста полужирным обрамите его звездочками **:
 
**Полужирный** 

4. Для создания ненумерованных списков используйте * в начале строки

   * элемент 1
   * элемент 2
   * элемент 3

5. Для создания нумерованных списков используйте цифры с точкой в начале строки

   1. Первый элемент
   2. Второй элемент
   3. Третий элемент

6. Чтобы зачеркнуть текст используйте ~:

~~заголовок~~

7. Добавление картинки

![walle](wall_e_robot_trava_tsvetok_99198_1920x1080.jpg)

8. Добавление GIF

![duck](duck.gif)


9. Добавление ссылки

[GitHub](https://github.com/)

## Ветки в git
Чтобы посмотреть все ветки:

* git branch

Для создания новой ветки с именем branch_name:

* git branch branch_name

Чтобы переместиться к ветке branch_name:

* git checkout branch_name

## Слияние веток и решение конфликтов

Чтобы слить информацию из ветки branch_name в текущую:

* git merge branch_name

В случае конфликта нужно удалить все лишние строки и оставить ту часть, которая нужна. Если необходимо, то можно отредактировать её.

## Удаление веток
Для того чтобы удалить ветку с именем branch_name:

* git branch -d branch_name

Удаление с игнорированием ошибок:

* git branch -D branch_name

## Как сделать pull request

1. Делаем fork интересуещего нас аккаунта.
2. Делаем git clone для нашей версии репозитория
3. Создаем ветку с предлагаемыми изменениями
4. Производим изменения только в этой ветке
5. Отправляем эти изменения на свой аккаунт (push)
6. В окне на github появляется возможность отправить pull request.

## Справка

Чтобы вызвать справку по команде, допишите тег:

>--help

Примеры применения тега:

> git add --help

> git branch --help




Дополнить файл с инструкцией по работе с git (второе домашнее задание) и направить pull request в этот репозиторий. Файл с инструкцией необходимо дополнить информацией о работе с удаленными репозиториями.

В системе подгрузить скриншот отправленного pull request

## Домашнее задание

Как сделать pull request

1. В github делаем fork интересуещего нас репозитория.
2. Делаем git clone (ссылка нашего репозитория)
3. Делаем необходимые изменения в скопированном файле
4. Сохраняем изменения (add, commit)
5. Отправляем эти изменения на свой аккаунт (push)
6. В github появится измененный файл и  возможность отправить pull request.

