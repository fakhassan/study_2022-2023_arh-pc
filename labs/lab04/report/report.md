---
# Front matter
title: "Шаблон отчёта по лабораторной работе 4"
subtitle: "Простейший вариант"
author: "хассан факи абакар"

# Generic otions
lang: ru-RU
toc-title: "Содержание"

# Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

# Pdf output format
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
### Fonts
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
## Misc options
indent: true
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
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

** 4.2.1. Базовые сведения о Markdown**

Чтобы создать заголовок, используйте знак #, например:

  .# This is heading 1
  .## This is heading 2
  .### This is heading 3
  .#### This is heading 4

This text is ** bold**.
Чтобы задать для текста курсивное начертание, заключите его в одинарные
звездочки:
This text is *italic*.

Чтобы задать для текста полужирное и курсивное начертание, заключите его
в тройные звездочки:
This is text is both ** * bold and italic***.

# Выполнение лабораторной работы

Описываются проведённые действия, в качестве иллюстрации даётся ссылка на иллюстрацию.

![Название рисунка](image/0.png){ #fig:001 width=70% }

![Установка TeX Live ](image/1.png){ #fig:0001 width=70% height=70%}

![zcat install-tl-unx.tar.gz | tar xf и cd install-tl-](image/2.png){ #fig:002 width=70% height=70%}

![cd install-tl-](image/2.png){ #fig:003 width=70% height=70%}

![конца Установка](image/3.png){ #fig:004 width=70% height=70%}

![xport/usr/local/texlive/2022/bin/x86_64-linux](image/4.png){ #fig:005 width=70% height=70%}

![wget](image/2018.png){ #fig:006 width=70% height=70%}

** crossref/releases/download/v0.3.13.0/pandoc-crossref-**
** Linux.tar.xz**

![sudo cp /tmp/pandoc-2.18/bin/pandoc /usr/local/bin/](image/5.png){ #fig:007 width=70% height=70%}

![C помощью команды ls](image/0.png){ #fig:001 width=70% height=70%}

# Выводы

В заключение можно сказать, что лаборатория позволяет разрабатывать отчеты с использованием легкого языка разметки Markdown.

# Список литературы{.unnumbered}
::: {#refs}
:::

