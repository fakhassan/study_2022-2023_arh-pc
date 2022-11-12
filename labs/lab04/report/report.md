---
## Front matter
title: "Шаблон отчёта по лабораторной работе 4"
subtitle: "Простейший вариант"
author: "хассан факи абакар"

## Generic otions
lang: ru-RU
toc-title: "Содержание"
**1. Цель работы**
**2.задание**
**3. Теоретическое введение**
**4 выполнение лабораторной работы**
**5 выводы**


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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Целью работы является освоение процедуры оформления отчетов с помощью
легковесного языка разметки Markdown.

# Задание

1. В соответствующем каталоге сделайте отчёт по лабораторной работе No 3
в формате Markdown. В качестве отчёта необходимо предоставить отчёты
в 3 форматах: pdf, docx и md.
2. Загрузите файлы на github.


# Теоретическое введение
**4.2.1. Базовые сведения о Markdown**

Чтобы создать заголовок, используйте знак #, например:
# This is heading 1
## This is heading 2
### This is heading 3
#### This is heading 4

This text is **bold**.
Чтобы задать для текста курсивное начертание, заключите его в одинарные
звездочки:
This text is *italic*.

Чтобы задать для текста полужирное и курсивное начертание, заключите его
в тройные звездочки:
This is text is both ***bold and italic***.

# Выполнение лабораторной работы

Описываются проведённые действия, в качестве иллюстрации даётся ссылка на иллюстрацию (рис. [-@fig:001])

![Название рисунка](image/placeimg_800_600_tech.jpg){ #fig:001 width=70% }
![Название рисунка](image/1)
**Установка TeX Live**

![Название рисунка](image/2)
**zcat install-tl-unx.tar.gz | tar xf и cd install-tl-**

![Название рисунка](image/2)
**cd install-tl-**

![Название рисунка](image/3)
**конца Установка**

![Название рисунка](image/4)
**xport PATH=$PATH:/usr/local/texlive/2022/bin/x86_64-linux**

![Название рисунка](image/2018.PNG)
**wget https://github.com/lierdakil/pandoc-**
**crossref/releases/download/v0.3.13.0/pandoc-crossref-**
**Linux.tar.xz**

![Название рисунка](image/5png)
**sudo cp /tmp/pandoc-2.18/bin/pandoc /usr/local/bin/**
**sudo cp /tmp/pandoc-crossref /usr/local/bin/**

![Название рисунка](image/00png)
**C помощью команды ls**
# Выводы

В заключение можно сказать, что лаборатория позволяет разрабатывать отчеты с использованием легкого языка разметки Markdown.

# Список литературы{.unnumbered}
::: {#refs}
:::
