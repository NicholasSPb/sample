# Команды Git

## Оглавление
[init](#init)  
[config](#config)  
[status](#status)  
[add](#add)  
[rm](#rm)  
[commit](#commit)  
[show](#show)  
[branch](#branch)  
[checkout](#checkout)  

## init

Инициализирует репозиторий git.

## config

Конфигурирование git.  
`git config --global alias.commitall '!git add .;git commit'` - создает алиас __commitall__,  
при вызове которого происходит индексирование всех файлов в рабочей директории и их закоммичивание.

## status

Показывает состояние файлов в рабочем каталоге: какие файлы изменены, проиндексированы или нет.

## add

Добавляет в индекс изменения для последующего коммита.  
Параметры:  
- __-A__ - индексирует все файлы в проекте;
- __.__ - аргумент, при использовании которого индексируются все файлы в текущей директории;
- __p__ - позволяет выборочно индексировать изменения в файлах.

## rm
Удаляет файлы из индекса и рабочей директории.  
Если вызвать с флагом _--cached_, то удаление происходит только из индекса.  
Параметры:  
- __r__ - рекурсивно.

## commit
Записывает изменения в репозиторий.  
Параметры:  
- __a__ - индексирует изменения всех отслеживаемых файлов, позволяет не вызывать отдельно __add__; 
- __m__ - для ввода краткого функционального сообщения о закоммиченных изменениях проекта.

## show

`git show <xxxx>(первые 4 символа хеша коммита) --pretty-fuller` - выводит в консоль закоммиченные изменнения.

## branch
Работа с ветками.

## checkout
Переключение между ветками.  
Параметры:  
- __b__ - создание новой ветки от текущей и переключение на нее.

[Официальная документация](https://git-scm.com/)