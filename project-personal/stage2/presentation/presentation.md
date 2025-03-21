---
## Front matter
lang: ru-RU
title: Презентация по 2 этапу индивидуального проекта
subtitle: Основы информационной безопасности
author:
  - Чувакина М. В.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 17 марта 2025

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Чувакина Мария Владимировна
  * студентка группы НКАбд-03-23
  * Российский университет дружбы народов
  * [1132236055@rudn.ru](mailto:1132236055@rudn.ru)
  * <https:/mvchuvakina.github.io/ru/>

:::
::: {.column width="30%"}


:::
::::::::::::::

## Цель

Приобретение практических навыков по установке DVWA.

# Выполнение лабораторной работы

## 1.1

Настройка DVWA происходит на нашем локальном хосте, поэтому нужно перейти в директорию `/var/www/html`. Затем клонирую нужный репозиторий GitHub

![Клонирование репозитория](image/1.png){#fig:001 width=70%}

## 1.2

Повышаю права доступа к этой папке до 777

![Изменение прав доступа](image/2.png){#fig:002 width=70%}

## 1.3

Чтобы настроить DVWA, нужно перейти в каталог `/dvwa/config` 

![Перемещение по директориям](image/3.png){#fig:003 width=70%}

## 1.4

Создаем копию файла, используемого для настройки DVWA `config.inc.php.dist` с именем `config.inc.php`.

![Создание копии файла](image/5.png){#fig:004 width=70%}

## 1.5

Изменяю данные об имени пользователя и пароле

![Редактирование файл](image/4.png){#fig:006 width=70%}

## 2.1

Запускаю mysql

![Запуск mysql](image/6.png){#fig:007 width=70%}

## 2.2

Авторизируюсь в базе данных от имени пользователя root. Создаем нового пользователя, используя учетные данные из файла config.inc.php

![Авторизация в базе данных](image/7.png){#fig:008 width=70%}

## 2.3

Теперь нужно пользователю предоставить привилегии для работы с этой базой данных

![Изменение прав](image/8.png){#fig:009 width=70%}

## 3.1

Необходимо настроить сервер apache2, перехожу в соответствующую директорию

![Перемещение между директориями](image/9.png){#fig:010 width=70%}

## 3.2

В файле параметры allow_url_fopen и allow_url_include должны быть поставлены как `On` 

![Редактирование файла](image/10.png){#fig:012 width=70%}

## 3.3

Запускаем службу веб-сервера apache и проверяем, запущена ли служба 

![Запуск apche](image/11.png){#fig:013 width=70%}

## 4.1

Мы настроили DVWA, Apache и базу данных, поэтому открываем браузер и запускаем веб-приложение, введя 127.0.0/DVWA 

![Запуск веб-приложения](image/12.png){#fig:014 width=70%}

## 4.2

Прокручиваем страницу вниз и нажимем на кнопку `create\reset database`

!["Создание базы данных"](image/13.png){#fig:015 width=70%}

## 4.3

Авторизуюсь с помощью предложенных по умолчанию данных 

![Авторизация](image/14.png){#fig:016 width=70%}

## 4.4

Оказываюсь на домшней странице веб-приложения, на этом установка окончена 

![Домашняя страница DVWA](image/15.png){#fig:017 width=70%}



## Вывод

Приобрела практические навыки по установке уязвимого веб-приложения DVWA.

# Спасибо за внимание
:::

