# Инструкция по работе с Git 

![Альтернативный текст](github.jpg)

## Начальные настройки и установки

*git config --global user.name «Ваше имя английскими буквами»  например: Konstantin*

*git config --global user.email ваша почта@example.com*

*git init* – **инициализация локального репозитория**

*git status* – **получить информацию от git о его текущем состоянии**

*git add* – **добавить файл или файлы к следующему коммиту**

*git commit -m “message”* – **создание коммита**.

*git log* – **вывод на экран истории всех коммитов с их хеш-кодами**

*git checkout* – **переход от одного коммита к другому**

*git checkout* master – **вернуться к актуальному состоянию и продолжить работу**

*git diff* – **увидеть разницу между текущим файлом и закоммиченным файлом**

## Работа с ветками

*git branch* – **посмотреть список веток в репозитории**

*git branch <название ветки>* – **создать новую ветку**

*git checkout <название ветки>* – **переход к другой ветке**

*git branch -d <название ветки>* – **удалить ветку**

## Работа с удаленными репозиториями

*git clone <ссылка>* - **команда для загрузки удаленного репозитория**

*git push* - **команда для отправки изменений из локального репозитория в удаленный**

*git pull* - **команда для подгрузки изменений из удаленного репозитория в локальный**




# Функции языка разметки Markdown

## Заголовки

Язык поддерживает 2 стиля обозначения заголовков: подчеркивание и выделение символом («#»). Выделение заголовков с помощью подчеркивания производится знаками равенства («=») в случае, если заголовок первого уровня, и дефисами («-») в случае, если заголовок второго уровня. Количество знаков подчеркивания не ограничивается. При выделении заголовков с помощью символа («#») используется от одного до шести данных символов, которые устанавливаются в начале строки (перед заголовком). В данном случае количество символов соответствует уровню заголовка. Кроме того, заголовок возможно снабдить закрывающимися символами («#»), хотя это и не является обязательным. Количество закрывающихся символов не обязано соответствовать количеству начальных символов. Уровень заголовка определяется по количеству начальных символов.
Заголовки первого и второго уровней, выполненные с помощью подчеркивания, выглядят следующим образом:

Заголовок первого уровня
========================

Заголовок второго уровня
-------------------------


Заголовки первого, третьего и шестого уровней, выполненные с помощью символа («#»), выглядят следующим образом:

#  Заголовок первого уровня
### Заголовок третьего уровня
###### Заголовок шестого уровня


## Выделение текста

Чтобы выделить текст курсивом необходимо обрамить его здездочками (*) или знаком нижнего подчеркивания (_). Например, *вот так* или _вот так_.

Чтобы выделить текст полужирным, необходимо обрамить его двойными звездочками (**) или двойным знаком нижнего подчеркивания (__). Например, **вот так** или __вот так__.

Альтернативные способы выделения текста жирным или курсивом нужны для того чтобы мы могли совмещать оба этих способа. Например, _текст может быть выделен курсивом и при этом быть **полужирным**_.

## Списки

Чтобы добавить ненумерованные списки, необходимо пункты выделить звездочкой (*) или знаком +. Например, вот так:
* Элемент 1
* Элемент 2
* Элемент 3
+ Элемент 4

Чтобы добавить нумерованные списки, необходимо пункты просто пронумеровать. Например, вот так:
1. Первый пункт
2. Второй пункт

## Цитаты

Для обозначения цитат в языке Markdown используется знак «больше» («>»). Его можно вставлять как перед каждой строкой цитаты, так и только перед первой строкой параграфа. Также синтаксис позволяет создавать вложенные цитаты (цитаты внутри цитат). Для их разметки используются дополнительные уровни знаков цитирования («>»). Цитаты могут содержать всевозможные элементы разметки. Цитаты выглядят следующим образом: 
>Это пример цитаты,
>в которой перед каждой строкой
>ставится угловая скобка.

Вложение цитаты в цитату выглядит следующим образом:
> Первый уровень цитирования
>> Второй уровень цитирования
>>> Третий уровень цитирования
>
>Первый уровень цитирования

# Горизонтальные линии (разделители)

Для того чтобы создать горизонтальную линию с использованием синтаксиса языка Markdown, необходимо поместить три (или более)дефиса или звездочки на отдельной строке текста. Между ними возможно располагать пробелы. Горизонтальные линии в Markdown выглядят следующим образом:

Первая часть текста, который необходимо разделить
***
Вторая часть текста, который необходимо разделить

# Ссылки

Markdown поддерживает два стиля оформления ссылок:

*Гиперссылка, с немедленным указанием адреса (внутритекстовая)*;
*Гиперссылка, подобная сноске*.

Подразумевается, что помимо URL-адреса существует еще текст ссылки. Он заключается в квадратные скобки. Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо поместить URL-адрес. В них же возможно расположить название, заключенное в кавычки, которое будет отображаться при наведении, но этот пункт не является обязательным.

[пример](http://example.com/ "Необязательная подсказка")

# Изображения

В Markdown существует 2 способа вставки изображений в документ:

1. С помощью непосредственного указания URL-адреса изображения. Синтаксис данной команды выглядит следующим образом:

![Альтернативный текст](111.jpg)

### Иными словами, он состоит из следующих элементов:

* восклицательный знак;
* квадратные скобки, в которых указывается альтернативный изображению текст (он станет содержимым атрибута в элементе img);
* круглые скобки, содержащие URL-адрес или относительный путь изображения, а также (необязательно) всплывающую подсказку, заключённуе в двойные или одиночные кавычки.
