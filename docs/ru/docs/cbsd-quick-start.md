# CBSD Quick Start Guide

## Инициализация

Инструкция для быстрого начала использования CBSD

Установить CBSD из портов или pkg

```
make -C /usr/ports/sysutils/cbsd install
pkg install -y cbsd
```

Настроить рабочий каталог в /usr/jails и произвести инициализацию:

```
env workdir=/usr/jails /usr/local/cbsd/sudoexec/initenv
```
В большинстве случаев подойдут параметры по-умолчанию, просто нажимайте Enter если согласны с ними

Если возникли вопросы по индивидуальной настройки, просмотрите страницу Первичная инициализация

## Создание и запуск jail

Запустить конфигуратор создания контейнера

```
cbsd jconstruct-tui
```

Запустить контейнер

```
cbsd jstart
```


## Создание и запуск bhyve

Запустить конфигуратор создания виртуальной машины

```
cbsd bconstruct-tui
```

Запустить виртуальную машину

```
cbsd bstart
```
