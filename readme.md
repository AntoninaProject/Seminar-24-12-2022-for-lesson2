# Инструкция по работе с Git и ветками

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
Для перемещения на предыдущие коммиты используется комманда *git checkout*. Для этого необходимо в журнале изменений, как показано в предыдущей части, найти необходимый коммит и его номер. После чего в терминале с папкой-репозиторием написать комманду *git checkout <номер коммита>*. После применения этой комманды, вы попадёте в состояние *Detached head*, в котором никакие изменения фиксироваться не будут. Для возврата в обычное состояние необходимо написать комманду *git checkout master*.  

## Ветки в Git
### Создание веток в Git
Чтобы посмотреть список веток, используем комманду *git branch*. Если хотим создать новую ветку, то к команде *git branch* добавляем название новой ветки. Не забываем переключиться на созданную ветку. Чтобы переключиться на созданную ветку используем комманду *git checkout <название ветки>*. После внесения изменений в новой ветке делаем обязательно коммит. Для возвращения в основную ветку используем комманду *git checkout master*.
Для создания новой ветки используется комманда *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать команду *git branch <название ветки>*.
### Просмотр списка веток
Для просмотра списка веток используется команда *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать комманду *git branch*. Зелёным цветом с символом **звёздочка** будет выделена текущая ветка. 

## Слияние веток и разрешение конфликтов
Для слияния веток используем комманду *git merge <имя ветки, которую необходимо слить с текущей>*. Если необходимо посмотреть дерево веток, то используем комманду *git log --graph*.
Разрешение конфликтов осуществляется после слияния веток. Для этого необходимо после возникновения конфликта вручную удалить все технические символы и привести текст к нужному нам значению, далее сделать коммит всех изменений. 

## Удаление веток
Для удаления веток используем комманду *git branch -d <имя ветки, которую хотим удалить>*.
