---
## Front matter
title: "Отчет по лабораторной работе №1"
subtitle: "Архитектура ОС"
author: "Михальский Кирилл Алексеевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Приобретение практических навыков установки ОС на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Задание

1. Установка Virtual Box
2. Установка ОС
3. После установки ОС
4. Настройка раскладки клавиатуры
5. Установка програмного оеспечения для создания документации

# Теоретическое введение

Виртуальная машина - компьютерная программа, имитирующая настоящий компьютер, который существует внутри основной ОС пользователя.

# Выполнение лабораторной работы

1. Сама VBox уже установлена на моем устростве. Для начала работы необходимо произвести все настройки.
Добавляю новую виртуальную машину. Указываю скачаннный ISO файл. Задаю имя.

![Настройка 1](image/1.png){#fig:001 width=70%}

Указываю выделяемый размер ОП. Указываю поддержку EFI.

![Настройка 2](image/2.png){#fig:002 width=70%}

Указываю выделяемый размер ЖД.

![Настройка 3](image/3.png){#fig:003 width=70%}

Включаю 3Д ускорение.

![Настройка 4](image/4.png){#fig:004 width=70%}

2. Запускаю виртуальную машину и пишу в терминале команду liveinst.

![liveinst](image/5.png){#fig:005 width=70%}

Создаю пользователя root.

![Установка 1](image/6.png){#fig:006 width=70%}

Указываю настройки в меню установки.

![Установка 2](image/7.png){#fig:007 width=70%}

3. Захожу в ОС.

![Вход](image/8.png){#fig:008 width=70%}

Переклчаюсь в супер пользователя. Обновляю средства разработки

![Обновление 1](image/9.png){#fig:009 width=70%}

Обновляю все пакеты.

![Обновление 2](image/10.png){#fig:010 width=70%}

Устанавливаю консоль.

![Установка](image/11.png){#fig:011 width=70%}

Устанавливаю dnf - automatic.

![Скачивание](image/12.png){#fig:012 width=70%}

Запускаю таймер со стандартной конфигурацией.

![Таймер](image/13.png){#fig:013 width=70%}

Меняю значение с enforcing на permissive для отключения SELinux.

![Отключение](image/14.png){#fig:014 width=70%}

Создаю и меняю конфигурационный файл.

![Конфигурация 1](image/15.png){#fig:015 width=70%}

Редактирую конфигурационный файл.

![Конфигурация 2](image/16.png){#fig:016 width=70%}

Установил pandoc, pandoc-crossref, texlive-scheme-full.

![Проверка](image/17.png){#fig:017 width=70%}

Домашняя работа:

Вывел все нужные атрибуты через поиск.

![ДЗ](image/18.png){#fig:018 width=70%}
 

# Выводы

Приобрел практические навыки по установки ОС на виртуальную машину, научился настраивать базовые сервисы ОС.

# Список литературы{.unnumbered}

::: {#refs}
:::
