---
## Front matter
title: "Шаблон отчёта по лабораторной работе"
subtitle: "Простейший вариант"
author: "хассан факи"

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
Освоение процедуры компиляции и сборки программ, написанных на ассем-
блере NASM.

# Задание
1. В каталоге ~/work/arch-pc/lab05 с помощью команды cp создайте копию
файла hello.asm с именем lab5.asm
2. С помощью любого текстового редактора внесите изменения в текст про-
граммы в файле lab5.asm так, чтобы вместо Hello world! на экран выво-
дилась строка с вашими фамилией и именем.
3. Оттранслируйте полученный текст программы lab5.asm в объектный
файл. Выполните компоновку объектного файла и запустите получивший-
ся исполняемый файл.
4. Скопируйте файлы hello.asm и lab5.asm в Ваш локальный репозиторий
в каталог ~/work/study/2022-2023/"Архитектура компьютера"/arch-
pc/labs/lab05/. Загрузите файлы на Github


# Теоретическое введение
Основными функциональными элементами любой электронно-вычислительной
машины (ЭВМ) являются центральный процессор, память и периферийные
устройства (рис. 5.1).
Взаимодействие этих устройств осуществляется через общую шину, к которой
они подключены. Физически шина представляет собой большое количество про-
водников, соединяющих устройства друг с другом. В современных компьютерах
проводники выполнены в виде электропроводящих дорожек на материнской
(системной) плате.

**Ассемблер и язык ассемблера**
Язык ассемблера (assembly language, сокращённо asm) — машинно-
ориентированный язык низкого уровня. Можно считать, что он больше любых
других языков приближен к архитектуре ЭВМ и её аппаратным возможностям,
что позволяет получить к ним более полный доступ, нежели в языках высокого
уровня, таких как C/C++, Perl, Python и пр

**Процесс создания и обработки программы на языке**
Процесс создания ассемблерной программы можно изобразить в виде следу-
ющей схемы


# Выполнение лабораторной работы

Создайте каталог для работы с программами на языке ассемблера NASM (рис1. [-@fig:001])
![Создайте каталог для работы команды](image/1.jpg){#fig:001 width=70%}

откройте этот файл с помощью любого текстового редактора (рис2. [-@fig:002])
![gedit hello.asm](image/2.jpg){ #fig:002 width=70%}

откройте этот файл с помощью любого текстового редактора, например, gedi (рис3. [-@fig:003])
![ассемблерная программа под названием nasm](image/3.jpg){#fig:003 width=70%}

Расширенный синтаксис командной строки NASM (рис4[-@fig:004])
![Выполните следующую команду:](image/4.jpg){#fig:004 width=70%}

Компоновщик LD (рис5[-@fig:005])
![Запуск исполняемого файла](image/5.jpg){#fig:005 width=70%}

В каталоге ~/work/arch-pc/lab05 с помощью команды cp создайте копию
файла hello.asm с именем lab5.asm (рис9[-@fig:009])
![проверьте наш файл с помощью команды ls ](image/9.jpg){#fig:009 width=70%}

С помощью любого текстового редактора внесите изменения в текст про-
граммы в файле lab5.asm так, чтобы вместо Hello world! на экран выво-
дилась строка с вашими фамилией и именем (рис6[-@fig:006])
![ текст программы в файле lab5.asm](image/6.jpg){#fig:006 width=70%}

Скопируйте файлы hello.asm и lab5.asm в Ваш локальный репозиторий
в каталог ~/work/study/2022-2023/"Архитектура компьютера"/arch-
pc/labs/lab05/. Загрузите файлы на Github (рис8[-@fig:008])
![ Скопируйте файлы hello.asm](image/8.jpg){ #fig:008 width=70% }





# Выводы

в заключение эта лабораторная позволила нам компилировать и собирать программы на ассемблере NASM.

# Список литературы{.unnumbered}

::: {#refs}
:::
