# Development of software modules

Лабораторные работы по предмету "Разработка программных модулей"

Лабораторные работы импортированы в качестве подмодулей [git submodules](https://git-scm.com/book/ru/v2/%D0%98%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-Git-%D0%9F%D0%BE%D0%B4%D0%BC%D0%BE%D0%B4%D1%83%D0%BB%D0%B8)


## Дополнительные инструкции

### Добавление репозитория с заданием
Добавление репозитория с заданием 
```shell
git submodule add <Ссылка на репозиторий> <Наименование директории>
```

Например:
```shell
git submodule add https://github.com/ShlyapnikEgoist/dosm_lab15_task1 lab15_task1
```

### Получение изменений подмодуля из удалённого репозитория
Если вы хотите проверить наличие изменений в подмодуле, 
перейдите в его каталог и выполните git fetch, 
а затем git merge для обновления локальной версии отслеживаемой ветки.

```shell
$ git fetch
From https://github.com/chaconinc/DbConnector
   c3f01dc..d0354fc  master     -> origin/master
$ git merge origin/master
Updating c3f01dc..d0354fc
Fast-forward
 scripts/connect.sh | 1 +
 src/db.c           | 1 +
 2 files changed, 2 insertions(+)
```