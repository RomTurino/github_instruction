# Инструкиция по пользованию github

# Инструкция для работы с Git и удалёнными репозиториями # 

**Что такое Git?**

Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

**Подготовка репозитория**

Для создание репозитория необходимо выполнить команду *git init* в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка *.git)*

**Создание коммитов**

__Git add__

Для добавления измений в коммит используется команда *git add.* Чтобы использовать команду *git add* напишите *git add* <имя файла>

**Создание коммитов**

Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit.* Выполняется она так: *git commit -m* "<сообщение к коммиту>. Все файлы для коммита должны быть ДОБАВЛЕНЫ и сообщение к коммиту писать *__ОБЯЗАТЕЛЬНО__*.

**Перемещение между сохранениями**

Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

**Журнал изменений**

Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

** Ветки в *Git* **

**Создание ветки**

Для того, чтобы создать ветку, используется команда *git branch.* Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

**Слияние веток**

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge*

**Удаление веток**

Для удаления ветки ввести команду *"git branch -d 'name branch'"*

**Создание картинов**

![pictures](https://thumb.tildacdn.com/tild6336-6565-4834-b433-616638643930/-/resize/960x/-/format/webp/2_git_fetch_pull_pus.png)

!\[text]\(name.gif)

**Ветки**

Ветки нужны, чтобы несколько программистов могли вести работу над одним и тем же проектом или даже файлом одновременно, при этом не мешая друг другу.

Кроме того, ветки используются для тестирования экспериментальных функций: чтобы не повредить основному проекту, создается новая ветка специально для экспериментов. Если эксперимент удался, изменения с экспериментальной ветки переносятся на основную, если нет – новая ветка попросту удаляется, а проект остается нетронутым.

Больше информации [тут](https://smartiqa.ru/courses/git/lesson-3).

**Просмотр старых коммитов и перемещение указателя HEAD**

Итак, пришло время разобраться, каким образом можно перемещать HEAD (и другие указатели тоже) и что это дает. Для начала нужно прояснить несколько важных аспектов, которые мы уже упоминали, но не обращали ваше внимание на них:

1. Весь репозиторий – это древовидный граф, ноды которого – наши коммиты, а ребра – родительские отношения между коммитами.
2. *HEAD* – это указатель (то есть ссылка на один из коммитов), главное назначение которого - определять, в каком состоянии находится рабочая копия. На какой коммит указывает *HEAD* – в таком состоянии файлы и находятся в рабочей области.
**Ветки**

Ветки нужны, чтобы несколько программистов могли вести работу над одним и тем же проектом или даже файлом одновременно, при этом не мешая друг другу.

Кроме того, ветки используются для тестирования экспериментальных функций: чтобы не повредить основному проекту, создается новая ветка специально для экспериментов. Если эксперимент удался, изменения с экспериментальной ветки переносятся на основную, если нет – новая ветка попросту удаляется, а проект остается нетронутым.

**Просмотр старых коммитов и перемещение указателя HEAD**

Итак, пришло время разобраться, каким образом можно перемещать HEAD (и другие указатели тоже) и что это дает. Для начала нужно прояснить несколько важных аспектов, которые мы уже упоминали, но не обращали ваше внимание на них:

1. Весь репозиторий – это древовидный граф, ноды которого – наши коммиты, а ребра – родительские отношения между коммитами.
2. *HEAD* – это указатель (то есть ссылка на один из коммитов), главное назначение которого - определять, в каком состоянии находится рабочая копия. На какой коммит указывает *HEAD* – в таком состоянии файлы и находятся в рабочей области.
**Просмотр старых коммитов и перемещение указателя HEAD**

Итак, пришло время разобраться, каким образом можно перемещать HEAD (и другие указатели тоже) и что это дает. Для начала нужно прояснить несколько важных аспектов, которые мы уже упоминали, но не обращали ваше внимание на них:

1. Весь репозиторий – это древовидный граф, ноды которого – наши коммиты, а ребра – родительские отношения между коммитами.
2. *HEAD* – это указатель (то есть ссылка на один из коммитов), главное назначение которого - определять, в каком состоянии находится рабочая копия. На какой коммит указывает *HEAD* – в таком состоянии файлы и находятся в рабочей области.

**Откат коммитов. Команда _git revert_.**

Пожалуй одна из самых важных частей в изучении Git – научиться откатываться к предыдущим коммитам. Смысл отката мы обсуждали в предыдущих уроках: ваш проект может перестать работать по непонятным вам причинам после внесения некоторых изменений в код, в таком случае важно быстро вернуть все к рабочему состоянию и только потом заниматься поиском ошибки. В этом-то случае нам и поможет откат коммитов и команда *git revert*.

Суть работы данной команды в том, что она создает новый коммит, который отменяет изменения внесенные в переданном коммите (последовательности коммитов).

**Ручное разрешение конфликта**

Видим, что *Git* оставил нам пометки, чтобы нам было проще устранять конфликт:
Текст до <<<<<<< *HEAD* – это общая часть двух файлов, она не конфликтует. В нашем случае оба файла имеют одинаковую первую строку: - *This is documentation*
Текст между <<<<<<< *HEAD* и ======= – это конфликтующее содержимое файла, на который указывает HEAD, то есть файла из целевой ветки. В нашем случае это вторая строка, именно она переписывается изменениями из ветки develop.
Все, что находится между ======= и >>>>>>> *develop* – это содержимое файла из ветки *develop*. В нашем случае это вторая и третья строки: - *New feature info и - It has lots of info*.

3.2. Выбор одного из двух файлов
Если вы точно знаете, что вам нужно оставить только один из двух конфликтных файлов (вся информация из другого файла при этом потеряется), можно сказать об этом Git:
Выполните git checkout --ours Docs.md, чтобы выбрать файл ветки main (то есть целевой ветки)
Либо git checkout --their Docs.md, чтобы выбрать файл из ветки develop (то есть сливаемой ветки).
Эта команда скопирует в docs.md из рабочей копии содержимое одного из конфликтных файлов. То есть Git полностью заменит файл в рабочей копии выбранным вами файлом.
Git Bash

**Разрешим конфликт выбором файла из коммита, к которому мы откатываемся.**

* git checkout --their Docs.md
Updated 1 path from the index
Поздравляю, теперь конфликт разрешен! Кстати, если сейчас выполнить команду git status, нас ждет необычный вывод.

**Что такое удаленный репозиторий**

Удаленный (иногда говорят "внешний") репозиторий – это версии вашего проекта, сохраненные на удаленном сервере. Доступ к репозиторию на таком сервере может осуществляться по интернету или по локальной сети.
Удаленный репозиторий – полноценный репозиторий, ничем не отличающийся от локального. У удаленного репозитория есть собственные ветки, собственный указатель HEAD, своя история коммитов и так далее.

Если мы подключим удаленный репозиторий к своему локальному, то у нас появятся копии всех ссылочных объектов удаленного репозитория. То есть, например, у удаленного репозитория есть ветка main, а у нас будет копия этой ветки – origin/main. Все такие ссылочные объекты (указатели, ветки и теги) удаленного репозитория хранятся почти там же, где и у локального – в директории .git/refs/remotes/<имя_удаленного_репозитория>.

**Настройка подключения удаленного репозитория (сто процентов).**

Необходимость подключить удаленный репозиторий к уже существующему локальному возникает в ситуациях, когда вы решаете выгрузить уже написанный код на удаленный сервер. Это нужно, чтобы другие разработчики смогли получить к нему доступ или чтобы вы сами могли заниматься разработкой с нескольких компьютеров (например, домашнего и рабочего).

