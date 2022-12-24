# Инструкция по работе с Git

## Что такое git?
**Git** - это наиболее популярная реализация распределённой системы контроля версий. Самая популярная реализация **Git** -  это [GitHub](https://github.com/)

## Подготовка репозитория
Для создания репозитория используется команда *git init*. Для этого необходимо в терминале перейти в пустую папку, где в будущем будет репозиторий. Затем в терминале с папкой написать команду *Git init*

## Создание коммитов

### Добавление файла к коммиту
Для добавления файла к будущему коммиту используется команда *git add*. Для этого в терминале с папкой-репозиториейм необходимо написать *git add <название файла>*.

### Создание коммита
Для создания коммита используется комманда *git commit*. Для этого в терминале с папкой репозитория необходимо написать *git commit -m <сообщение к коммиту>*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО!!!***.

##  Журнал изменений
Для просмотра журнала изменений используется комманда *git log*. Для этого в терминале с папкой-репозиторием необходимо написать *git log*. 

## Перемещение между коммитами
Для перемещения на предыдущие коммиты используется комманда *git checkout"*. Для этого необходимо в журнале изменений, как показано в предыдущей части, найти необходимый коммит и его номер. После чего в терминале с папкой-репозиторием написать комманду *git checkout <номер коммита>*. После применения этой комманды, вы попадёте в состояние "Detached head", в котором никакие изменения фиксироваться не будут. Для возврата в обычное состояние необходимо написать комманду *git checkout master"*.  

## Ветки в Git

## Слияние веток и разрешение конфликтов

## Удаление веток