# Инструкция по работе с Git и ветками

## Что такое Git?

Git - одна из реализаций распределенных систем контроля версий, позволяющяя организовать версионность, как локально, так и на удаленном сервере. Самая популярная платформа реализующая *Git*, - [GitHub](https://github.com)

Git (произн. «гит») — распределённая система управления версиями файлов. Проект был создан Линусом Торвальдсом для управления разработкой ядра Linux.

## Подготовка репозитория

Для создания папки репозитория необходимо открыть эту папку в терминале и написать команду *git init* , после чего в этой папке создастся скрытая папки *.git* , и таким образом папка станет репозиторием.

## Что такое Удаленный репозитрий

Удалённый репозиторий — это модификация проекта, которая хранится в интернете или ещё где-то в сети. Удалённый репозиторий обычно доступен для вас либо только на чтение, либо на чтение и запись. Совместная работа включает в себя помещение (push) и получение (pull) данных и из них тогда, когда нужно обменяться результатами работы.

## Отображение удалённых репозиториев

Чтобы просмотреть какие удалённые серверы у вас уже настроены, следует выполнить команду *git remote*.

### Создание фиксаций

Для создания фиксации используется команда *git commit*. Для этого в термминале с папкой-репозиторием необходимо написать команду *git commit -m <сообщение к коммиту>*. Сообщение к коммиту писать **ОБЯЗАТЕЛЬНО**.

### Добавление файла к "сохранению"

Для того чтобы добавить файл к сохранению, необходимо использовать команду *git add*.  В терминале с открытой папкой-репозиторием необходимо написать *git add <название файла>*, и этот файл добавится к "сохранению"

## Журнал изменений

Для просмотра истории изменений используется команда *git log*. Для этого  в терминале с папкой-репозиторием необходимо написать *git log*, и Вы увидите список всех коммитов в этой ветке с описанием: имени, электронной почты, сообщением к комиту и номер коммита.

## Перемещение между коммитами

Для перемещения между коммитами используется команда *git checkout*. Для этого в терминале с мапкой-репозиторием необходимо написать *git checkout <номер коммита>*. Номер коммита берется из журнала изменений ветки.

## Что такое ветка

Ветка (или branch) — это своеобразное "место" разработки.

## Ветки в Git

### Создание ветки
Для того чтобы создать новую ветку, используется команда *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать *git branch <название ветки>* и таким образом создастся новая ветка, но Вы останитесь в исходной.

### Просмотр списка веток

Для того, чтобы просмотреть список веток в локальном репозитории, используется команда *git branch*. Для этого  в терминале с папкой-репозиторием напишите *git branch*, и тогда Вы увидите список всех Ваших локальных веток.
Зеленым цветом будет выделена ветка, на которой вы сейчас стоите. Флаг *-а* позволяет посмотреть все ветки, в том числе и в удаленном репозитории.

### Переключене между ветками
Для того, чтобы переключится между ветками, используется комманда *git checkout*. Для этого в терминале с папкой-репозиторием необходимо вписать *git checkout <название ветки>*, и тогда Вы перейдете в указанную ветку. Для переключения между ветками, ветка должна **СУЩЕСТВОВАТЬ**, и в текущей ветке не должно быть активных изменений.

## Слияние веток и разрешение конфликтов

Для слияния веток используется команда *git merge*. Для этого  в терминале с папкой-репозиторием необходимо написать *git merge (*название ветки*)*, после чего мы можем увидить стратегию, по которой произошло слияние:

- Fast - forward
- Merge made by "ort" strategy
- CONFLICT "КОНФЛИКТИТСТЕЙТ"

В ручном режиме устраняем конфликт и сохраняем файл.

## Удаление веток

Для удаления веток используется команда *git branch -d*. Для этого  в терминале с папкой-репозиторием необходимо написать *git branch -d <*название ветки*>.
