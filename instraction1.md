# Инструкция по языку MarkDown

## Немного теории по оформлению

Что значит символ в начале текста "#"? Это уровни заголовков.

"#"-Это заголовок 1-го уровня

"##"-Это заголовок 2-го уровня

"###"-Это заголовок 3-го уровня

Пример:

# Заголовок 1-го уровня
```sh
# Заголовок 1-го уровня
``` 

## Заголовок 2-го уровня
```sh
## Заголовок 2-го уровня
``` 
### Pаголовок 3-го уровня
```sh
### Pаголовок 3-го уровня
``` 

### Стилизации текста:
1. Полужирный необходимо текст заключить в нутри двойных символов звезда.
2. Курсив необходимо текст заключить в нутри одинарных символов звезда.

Пример:

**Полужирный стиль**
```sh
**Полужирный стиль**
``` 
*Стиль курсив*
```sh
*Стиль курсив*
``` 

### Цитирование (показано в примере №2):
1. ">"- Первый уровень
2. ">>"- Втрой уровень

Пример:
> Первый уровень
```sh
> Первый уровень
``` 
>> Второй уровень
```sh
>> Второй уровень
``` 
### Списки:
1. Ненумерованный, текст начинается с *текст
2. Нумированный, текст начинается с цифры, точки а после текст

Пример

Ненумерованный список
* Лист 1
* Лист 2
* Лист 3
```sh
* Лист 1
* Лист 2
* Лист 3
``` 

Нумерованный список

1. Лист 1
2. Лист 2
3. Лист 3
```sh
1. Лист 1
2. Лист 2
3. Лист 3
``` 
## Что такое GIT
Git - Git - это консольная утилита, для отслеживания и ведения истории изменения файлов, в вашем проекте.

## Теперь перейдем к начальным командам
Для визуальности *определения и поянения будем писать в ситле курсив*, **команды будем отмечать в полужирном стиле**.

**git init** - *создает новый репозиторий Git. С ее помощью можно преобразовать существующий проект без управления версиями в репозиторий Git или инициализировать новый пустой репозиторий с расширением ".git".*

```Sh
git init <directory>
```

**git add** - *это первая команда в цепочке операций, предписывающей Git «сохранить» снимок текущего состояния проекта в истории коммитов. Когда **git add** используется как отдельная команда, она переносит ожидающие изменения из рабочего каталога в раздел проиндексированных файлов. <u>Однако на самом деле команда **git** add не оказывает существенного влияния на репозиторий </u>*

**git commit -m "Message"** -Команда git commit делает для проекта снимок текущего состояния изменений, добавленных в раздел проиндексированных файлов. Такие подтвержденные снимки состояния можно рассматривать как «безопасные» версии проекта — Git не будет их менять, пока вы явным образом не попросите об этом. Перед выполнением команды git commit необходимо использовать команду git add, чтобы добавить в проект («проиндексировать») изменения, которые будут сохранены в коммите
```sh
git commit -m "Message"
"Message" -текст, к примеру внесены опрделенные изменения с такого по такието линии
```
**git log** - *Благодаря данной команды можно просмотреть историю проекта, с целью узнать, кто и что сделал, откуда появились баги, и отменить изменения, вызвавшие проблемы.*

**git log --oneline**- *командой мы можем упростить информацию которая предоставляется консолью после набора команды **git log**.*

**git checkout**- *команда, обновляющая файлы в рабочем каталоге до совпадения с состоянием в индексе или в определенной ветке. Во вселенной Git данная команда имеет важную роль в управлении состоянием рабочего каталога и в переходе между разными снапшотами истории проекта*

```sh
Пример:

git checkout fa52ea9 
таким образом можно переключиться на состояние вплоть до первоначального состояния, в данном случае в самое начало.
```
Чтобы перейти на последнее состояние
```sh
git checkout 'master'
```
Таким образом мы можем перемещаться по зафиксированным состояниям.

# Практика №2.
## Как добавить картинку в Markdown
Это символ 2024 года
![Дракон](2024.jpg)

### Это апельсины

![orange](orange.png)