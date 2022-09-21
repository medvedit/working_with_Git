# Инструкция для работы с *Git* и удаленным репозиториями.
![Git](data:image/png;base64,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)
***
## ***Что такое Git...?***
+ ***Git*** - это одна из реализаций распространённых систем контроля версий, имеющая, как и локальные, так и удаленные репозитории. Является самой популярной реализацией систем контроля версий в мире.
***
## *Подготовка репозитория:*
Для создания репозитория необходимо выполнить команду ***\*git init\****
>Напишите команду: ***git*** пробел ***init***

В папке с репозиторием у Вас появится репозиторий, скрытая папка ***.git***

## *Просмотр состояния репозитория*:

Для того, что бы посмотреть состояние репозитория используется команда ***\*git status\****. Что бы увидеть были ли изменения в файлах, или их не было
>Напишите команду: ***git*** пробел ***status***

## *Фиксация состояния*:

Команда ***\*git add\**** перемещает из рабочей папки в область индексирования предназначенное для следующей фиксации содержимое. Для создания фиксации изменений в рабочем файле используется команда ***\*git add\****. Что бы зафиксировать изменения
>Напишите команду: ***git*** пробел ***add*** пробел ***<Имя файла>***

## *Создание коммитов*:

Для того, чтобы создать коммит(сохранение) необходимо выполнить команду ***\*git commit\****. Выполняется она так:
>Напишите команду: ***git commit*** пробел ***-m*** пробел ***"сообщение к коммиту"*** (обязательно в ковычках)


Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** (cmd+S для Мас) и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## *Журнал изменений, коммитов*:

Для того, чтобы посмтреть все сделанные сохранения в репозитории, используется команда ***\*git log\****. Для этого достаточно выполнить команду в папке с репозиторием: 

>***git*** пробел ***log***

## *Перемещение между сохранениями, коммитами*:

Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда ***\*git checkout\****. Используется она в папке с репозиторием следующим образом:
>***git checkout*** пробел ***<номер коммита>*** (достаточно первые три знака).

Для ввода номера коммита достаточно первых четырёх знаков.

## *Возврат в последнее соханённое состояние, не переходя в другу ветку, для продолжения работы* :

Для Этого используется команда :
>***git*** пробел ***checkout*** пробел ***<имя ветки>***


***

# Создание веток *git* :

## *Создание ветки* :

Для того, чтобы создать ветку, используется команда ***\*git branch\****. Делается это следующим образом в папке с репозиторием:
>***git*** пробел ***branch*** пробел ***<название новой ветки>***

## *Слияние веток* :

Для того чтобы дабавить ветку в текущую ветку используется команда :

>***git*** пробел  ***merge*** пробел ***<имя ветки\>***

## *Удаление веток* :

Для удаления ветки ввести команду:

>***git*** пробел ***branch*** пробел  ***-d*** пробел ***<имя ветки>***

***
***
***

### P.S.: *И в заключении хотелось бы добавить, что все команды, то , как я оформил этот текст, в каждом знаке выше изложенного - заслуга моих преподавателей!!! Это* [Ильнар Шафигуллин](https://gb.ru/users/teachers/3546003 "Преподаватель GeekBrains") *человек умеющий* ***"красиво разложить"*** *и* ***"грамитно преподать"***. *И* [Софья Главацкая](https://gb.ru/users/teachers/7524512 "Преподаватель GeekBrains")-*покарившая своей ***добратой, умением слушать, терпением*** в помощи нам, задающим иногда глуппые вопросы, студентам* [GeekBrains](https://gb.ru "IT-образование"). ***Спасибо!!!***

![GeekBrains](https://habrastorage.org/webt/82/ui/ik/82uiiktyk5fmbezropgye812p-4.png)
