xdd-bootstrap-1C
======

Шаблон каталогов и примеры автоматизированных инструментов
------

bootstrap full source template for Bussines Process Automation platform www.1C.com

Данный проект является шаблоном каталогов и шаблонов рабочего процесса для разработчика при переходе команды на стандарты промышленной разработки на платформе 1С:Предприятие

> TODO - добавить подробное описание каталогов

Использование
------

### подключение к Вашему проекту 

**команды подключения к новому проекту**

```sh
> git clone https://github.com/xUnitFor1C/xdd-bootstrap-1C.git ./PROJECTNAME
> cd ./PROJECTNAME
> git submodule init
> git submodule update
> cd .\utils\precommit1c\ && copy-to-hook.cmd && cd .\..\..\..\
```

Для Github (репозиторий должен существовать)

```sh
> git remote set-url origin git@github.com:USERNAME/PROJECTNAME.git
```

Для BitBucket (репозиторий должен существовать)	

```sh
> git remote set-url origin https://USERNAME@bitbucket.org/USERNAME/PROJECTNAME.git
```

И последнее

```sh
> git push -u origin --all
```

**команды подключение к существующему проекту**

```sh
> git remote add workflow https://github.com/xUnitFor1C/xdd-bootstrap-1C.git
> git fetch worklow

Используйте git-flow или программу Source-Tree для создания новой функциональности (например feature/new-project-dirs)


```sh
> git merge workflow/master 
```                                                      

в проекте не содержится стандартных файлов README или LICENCE, единственным файлом обязательным к использованию - является .gitsubmodules. Если вы используейте дополниельный подмодуль, то:

1. выполните git pull request workflow/master
2. воспользйтесь [Созданием требований на новую функциональность](https://github.com/xUnitFor1C/xdd-bootstrap-1C/issues/new)


Особенности рефакторинга каталогов существующего проекта под стандартный шаблон каталогов
------

### Доработка шаблона (для контрибьютеров yDD Community) или обновление новых шаблонных инструментов

1. используйте Git Issue или git pull request
2. для обновления: 

```sh
> git remote add workflow https://github.com/xUnitFor1C/xdd-bootstrap-1C.git
> git fetch workflow
> git merge workflow/master 
```

А если завтра "война"
------

когда компания 1С выпустит свою версию и интерпретацию стандартного шаблона каталогов и скриптов мы с помощью git tag и git verison, а может быть даже с помощью git fork учтем её стандарт


[Лицензия на использование](licences/LICENSE.XDD.BOOTSTRAP)
