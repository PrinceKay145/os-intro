---
# Front matter
lang: ru-RU
title: "Шаблон отчёта по лабораторной работе № 7"
subtitle: "Операционные Системы"
author: "Адебайо Ридануллахи Айофе"
std. number: "1032205020"
Group: "НКНбд-01-20"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
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

Ознакомление с инструментами поиска файлов и фильтрации текстовых данных. Приобретение практических навыков: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

# Задание

1. Осуществите вход в систему, используя соответствующее имя пользователя.
2. Запишите в файл file.txt названия файлов, содержащихся в каталоге /etc.
Допишите в этот же файл названия файлов, содержащихся в вашем домашнем каталоге.
3. Выведите имена всех файлов из file.txt, имеющих расширение .conf, после чего запишите их в новый текстовой файл conf.txt.
4. Определите, какие файлы в вашем домашнем каталоге имеют имена, начинавшиеся с символа c? Предложите несколько вариантов, как это сделать.
5. Выведите на экран (по странично) имена файлов из каталога /etc, начинающиеся с символа h.
6. Запустите в фоновом режиме процесс, который будет записывать в файл
~/logfile файлы, имена которых начинаются с log.
7. Удалите файл ~/logfile.
8. Запустите из консоли в фоновом режиме редактор gedit.
9. Определите идентификатор процесса gedit, используя команду ps, конвейер и фильтр grep. Можно ли определить этот идентификатор более простым способом?
10. Прочтите справку (man) команды kill, после чего используйте её для завершения процесса gedit.
11. Выполните команды df и du, предварительно получив более подробную информацию об этих командах, с помощью команды man.
12. Воспользовавшись справкой команды find, выведите имена всех директорий,имеющихся в вашем домашнем каталоге.


# Выполнение лабораторной работы

1. Вошёл в систему, используя соответствующее имя пользователя

2. Записал в файл file.txt названия файлов, содержащихся в каталоге /etc.

![файл](image/01.jpg)

3.  Вывел имена всех файлов из file.txt, имеющих расширение .conf, после чего запишите их в новый текстовой файл conf.txt.

![файл](image/03.jpg)

4. Три варианты с помощью ``ls``, ``find``, и также ``grep``.
- find 

![файл](image/4find.jpg)

- grep

![файл](image/4grep.jpg)

5. Вывел на экран (по странично) имена файлов из каталога /etc, начинающиеся с символа h.

![файл](image/5.jpg)

6. Запустил в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log.

![файл](image/6.jpg)

7. Удалил файл ~/logfile.

![файл](image/7.jpg)

8. Запустил из консоли в фоновом режиме редактор gedit.

![файл](image/8.jpg)

9. Определил идентификатор процесса gedit, используя команду ps, конвейер и фильтр grep

![файл](image/9.jpg)

10. Прочитал справку (man) команды kill, после чего использовал её для завершения процесса gedit.

![файл](image/10.jpg)

11. Выполнил команды df и du,с помощью команды man
- Команда df

![df](image/11df.jpg)

- Команда du

 ![df](image/11du.jpg)
 
12. Вывел имена всех директорий,имеющихся в вашем домашнем каталоге, с помощью ``find``.

![файл](image/12.jpg)

# Контрольные вопросы

1. stdin — стандартный поток ввода (по умолчанию: клавиатура), файловый дескриптор 0;
2. /> - открытие файла для перенаправления потока.
   />> - файл открывается в режиме добавления.
3. Конвейер (pipe) служит для объединения простых команд или утилит в цепочки,в которых результат работы предыдущей команды передаётся последующей. Синтаксис следующий:
команда 1 | команда 2
означает, что вывод команды 1 передастся на ввод команде 2
4.  Процессы в linux можно описать как контейнеры, в которых хранится вся информация о состоянии и выполнении программы. 
5. Process IDentifier, PID) — уникальный номер (идентификатор процесса. (GID) - обозначает группу, к которой относится пользователь.
6. Запущенные фоном программы называются задачами (jobs). Ими можно управлять с помощью команды jobs, которая выводит список запущенных в данный момент задач.
7. top - позволяет выводить информацию о системе, а также список процессов динамически обновляя информацию о потребляемых ими ресурсах.
Команда htop похожа на команду top по выполняемой функции: они обе показывают информацию о процессах в реальном времени, выводят данные о потреблении системных ресурсов и позволяют искать, останавливать и управлять процессами.
В программе htop реализован очень удобный поиск по процессам, а также их фильтрация.
8. Команда find используется для поиска и отображения имён файлов, соответствующих заданной строке символов.
Формат команды:
find путь [-опции]
Путь определяет каталог, начиная с которого по всем подкаталогам будет вестисьпоиск.
Пример:
Вывести на экран имена файлов из вашего домашнего каталога и его подкаталогов, начинающихся на f:
``find ~ -name "f*" -print``
где ~ — обозначение вашего домашнего каталога, -name — после этой опции указывается имя файла, который нужно найти, "f*" — строка символов, определяющая имя файла, -print — опция, задающая вывод результатов поиска на экран.
9. Можно ли по контексту (содержанию) найти файл используя комбинацию команд find и grep. ``find -type f -exec grep -H 'текстДляПоиска' ``
10. определить объем свободной памяти на жёстком диске можно с помощью``df -h``
11. Определить объем домашнего каталога можно командой ``du -s``
12. Для завершения процесса необходимо выполнить команду
``kill %номер задач``

# Выводы

Ознакомился с инструментами поиска файлов и фильтрации текстовых данных. Приобрел практических навыков: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.
