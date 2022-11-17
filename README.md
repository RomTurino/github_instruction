# инструкция по пользованию  GitHub

## Выделение текста
----------
ля добавления измений в коммит используется команда *git add*. Чтобы использовать команду git add напишите *git add <имя файла>*

чтобы выделить текст, полужирным необходдимо обрамить его двойными звездочками (**) или двойным знаком нижнего подчеркивания (__). например, **вот так** или __вот так__
Альтернативные стособы выделения текста жирным или курсивон нужны для того, чтобы мы могли совмещать оба этих способа. например, _текст может быть выделен курсовом и при этом быть **полужирным**_.

## Списки
-----------
Списки бывают нумерованными и ненумерованными. Если нам нужен нумерованный список, то мы просто пишем каждый элемент со своим номером на новой строке, а MarkDown сам его красиво оформит.
 Например, вот так:
1.	первый элемент
2.	второй элемент
3.	третий элемент

Если нам нужны ненумерованные списки, то мы вместо числа (номера элемента) можем поставить + или *. Например, вот так:
* Элемент
* Элемент
+ элемент

## Работа с изображениями
------------
чтобы вставить изображение в текст достаточно написать следующее:

\!\[описание картинки](адрес) 

![remember](commands.jpg)   -   эта картинка не видна в GitHub
или

![картинка с интернета](https://upload.wikimedia.org/wikipedia/commons/thumb/3/35/Tux.svg/340px-Tux.svg.png "Linux")


## ссылки
----
для того, чтобы сделать ссылку, надо написать:

\[описание ссылки](адрес)

например,

 [github](https://github.com/)

[yandex](https://yandex.ru)

[google](https://google.com)

## работа с таблицами
--------
чтобы создать таблицу,  используются всего два символа: вертикальная черта ( \| ) и дефис ( \- ). Дефисы работают примерно так же, как в случае с горизонтальной линией: отделяют заголовки от других строк, при этом количество символов значения не имеет. Вертикальная черта служит границей между столбцами. 

Например:
| цена (руб.) | количество  (шт.)|
| --| -- |
| 5 | 25 |
| 35 | 2 |
| 3 | 18 |



## цитаты 
цитаты отмечаются  значком (\>)
> работа и труд все перетрут 

## Экранирование
-------
 Чтобы спецсимволы не исчезали и не влияли на оформление, нужно использовать экранирование. Как и во многих других языках программирования, этим целям служит обратная косая черта (бэкслеш) ( \ )

например:

\*нет курсива\*

\*\*нет полужирного\*\* 
  
работа с ветками


## работа с GitHub
----------
### создание репозитория
---
Для размещения своего репозитория на GitHub надо:
1. Создать account на сервисе
2. в правом верхнем углу нажать "+", выбрать создать новый репозиторий, дать ему имя, остальные парабетры оставить "по умолчанию"
3. Дальше сервис проедложит 
* создать новый репозиторий
* переместить существующий репозиторий
* или импортировать код для любого другого репозитория

При этом, для каждого действия будут подсказан набор команд.

Команда *git push* Вносит изменения **из** ветки **удалённого** репозитория **в** текущую ветку **локального** репозитория

Команда *git pull* заpагружает все изменения локальной ветки в удалённый репозиторийю При этом, вместе с загрузкой происходит с merge версий.



Загружает историю из удалённого репозитория и объединяет её с локальной. pull = fetch + merge