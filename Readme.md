# Инструкция по работе с Git

## Что такое Git?

Git - одна из реализаций распределенных систем контроля версий, позволяющяя организовать версионность, как локально, так и на удаленном сервере. Самая популярная платформа реализующая *Git*, - [GitHub](https://github.com)

## Подготовка репозитория

Для создания папки репозитория необходимо открыть эту папку в терминале и написать команду *git init* , после чего в этой папке создастся скрытая папки *.git* , и таким образом папка станет репозиторием.

### Создание фиксаций

Для создания фиксации используется команда *git commit*. Для этого в термминале с папкой-репозиторием необходимо написать команду *git commit -m <сообщение к коммиту>*. Сообщение к коммиту писать **ОБЯЗАТЕЛЬНО**.

### Добавление файла к "сохранению"

Для того чтобы добавить файл к сохранению, необходимо использовать команду *git add*.  В терминале с открытой папкой-репозиторием необходимо написать *git add <название файла>*, и этот файл добавится к "сохранению"

### Просмотр состояния репозитория

Для просмотра состояния репозитория используется команда гит статус. В терминале с ткрытой папкой-репозиторием необходимо написать команду *git status*. В результате можно увидить следующие выводы:

1. On branch *** nothing to commit - это означает нет активных изменений

2. Untracked file - это означает, что имеются файлы, не отслеживаемые системой контроля версий
...

## Журнал изменений

Для просмотра истории изменений используется команда *git log*. Для этого  в терминале с папкой-репозиторием необходимо написать *git log*, и Вы увидите список всех коммитов в этой ветке с описанием: имени, электронной почты, сообщением к комиту и номер коммита.

## Перемещение между коммитами

Для перемещения между коммитами используется команда *git checkout*. Для этого в терминале с мапкой-репозиторием необходимо написать *git checkout <номер коммита>*. Номер коммита берется из журнала изменений ветки.

## Ветки в Git

## Слияние веток и разрешение конфликтов

## Удаление веток

Для удаления веток используется команда *git branch -d*. Для этого  в терминале с папкой-репозиторием необходимо написать *git branch -d <*название ветки*>.
