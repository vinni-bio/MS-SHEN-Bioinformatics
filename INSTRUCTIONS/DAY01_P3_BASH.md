# LEEBAO-BIOINFORMATICS

Интенсивный курс по биоинформатике для магистрантов ШЕН


## ДЕНЬ 01. ПРАКТИКА: командная строка

## СОДЕРЖАНИЕ

1. [Командная оболочка `BASH`](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#1-%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4%D0%BD%D0%B0%D1%8F-%D0%BE%D0%B1%D0%BE%D0%BB%D0%BE%D1%87%D0%BA%D0%B0-bash-bourne-again-shell)

   1А. [Основные команды](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#1a-%D0%BE%D1%81%D0%BD%D0%BE%D0%B2%D0%BD%D1%8B%D0%B5-%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B)  
   1Б. [Специальные символы в `BASH`](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#1%D0%B1-%D1%81%D0%BF%D0%B5%D1%86%D0%B8%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5-%D1%81%D0%B8%D0%BC%D0%B2%D0%BE%D0%BB%D1%8B-%D0%B2-bash)  
   1В. [Управление командной строкой `BASH` путем нажатия клавиш](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#1%D0%B2-%D1%83%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4%D0%BD%D0%BE%D0%B9-%D1%81%D1%82%D1%80%D0%BE%D0%BA%D0%BE%D0%B9-bash-%D0%BF%D1%83%D1%82%D0%B5%D0%BC-%D0%BD%D0%B0%D0%B6%D0%B0%D1%82%D0%B8%D1%8F-%D0%BA%D0%BB%D0%B0%D0%B2%D0%B8%D1%88)  
   1Г. [Переменные среды `BASH` (избранные)](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#1%D0%B3-%D0%BF%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D1%8B%D0%B5-%D1%81%D1%80%D0%B5%D0%B4%D1%8B-bash%D0%B8%D0%B7%D0%B1%D1%80%D0%B0%D0%BD%D0%BD%D1%8B%D0%B5)  
   1Д. [Символы подстановки (wildcards)](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#1%D0%B4-%D1%81%D0%B8%D0%BC%D0%B2%D0%BE%D0%BB%D1%8B-%D0%BF%D0%BE%D0%B4%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B8-wildcards)  
   
2. [УПРАЖНЕНИЯ](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2-%D1%83%D0%BF%D1%80%D0%B0%D0%B6%D0%BD%D0%B5%D0%BD%D0%B8%D1%8F)

   2А. [Вывод строки на экран](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2%D0%B0-%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4-%D1%81%D1%82%D1%80%D0%BE%D0%BA-%D0%B8-%D0%B7%D0%BD%D0%B0%D1%87%D0%B5%D0%BD%D0%B8%D0%B9-%D0%BF%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D1%8B%D1%85-%D0%BD%D0%B0-%D1%8D%D0%BA%D1%80%D0%B0%D0%BD)  
   2Б. [Перемещение и операции с директориями](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2%D0%B1-%D0%BF%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D1%89%D0%B5%D0%BD%D0%B8%D0%B5-%D0%B8-%D0%BE%D0%BF%D0%B5%D1%80%D0%B0%D1%86%D0%B8%D0%B8-%D1%81-%D0%B4%D0%B8%D1%80%D0%B5%D0%BA%D1%82%D0%BE%D1%80%D0%B8%D1%8F%D0%BC%D0%B8)  
   2В. [Просмотр истории команд](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2%D0%B2-%D0%BF%D1%80%D0%BE%D1%81%D0%BC%D0%BE%D1%82%D1%80-%D0%B8%D1%81%D1%82%D0%BE%D1%80%D0%B8%D0%B8-%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4)  
   2Г. [Создание и чтение файлов](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2%D0%B3-%D1%81%D0%BE%D0%B7%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B8-%D1%87%D1%82%D0%B5%D0%BD%D0%B8%D0%B5-%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2)  
   2Д. [Символы подстановки (wildcards)](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2%D0%B4-%D1%81%D0%B8%D0%BC%D0%B2%D0%BE%D0%BB%D1%8B-%D0%BF%D0%BE%D0%B4%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B8-wildcards)  
   2Е. [Вызов справки (help и man)](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2e-%D0%B2%D1%8B%D0%B7%D0%BE%D0%B2-%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BA%D0%B8-help-%D0%B8-man)  
   2Ë. [Удаление папок и файлов](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2%C3%AB-%D1%83%D0%B4%D0%B0%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BF%D0%B0%D0%BF%D0%BE%D0%BA-%D0%B8-%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2)  
   2Ж. [Подстановки команд и меры предосторожности для новичков](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2%D0%B6-%D0%BF%D0%BE%D0%B4%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B8-%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4-%D0%B8-%D0%BC%D0%B5%D1%80%D1%8B-%D0%BF%D1%80%D0%B5%D0%B4%D0%BE%D1%81%D1%82%D0%BE%D1%80%D0%BE%D0%B6%D0%BD%D0%BE%D1%81%D1%82%D0%B8-%D0%B4%D0%BB%D1%8F-%D0%BD%D0%BE%D0%B2%D0%B8%D1%87%D0%BA%D0%BE%D0%B2)  
   2З. [Проверка типа консоли](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2%D0%B7-%D0%BF%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D0%BA%D0%B0-%D1%82%D0%B8%D0%BF%D0%B0-%D0%BA%D0%BE%D0%BD%D1%81%D0%BE%D0%BB%D0%B8)  
   2И. [Скачивание файлов из сети](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2%D0%B8-%D1%81%D0%BA%D0%B0%D1%87%D0%B8%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2-%D0%B8%D0%B7-%D1%81%D0%B5%D1%82%D0%B8)  
   2Й. [Работа с файловыми строками](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2%D0%B9-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0-%D1%81-%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2%D1%8B%D0%BC%D0%B8-%D1%81%D1%82%D1%80%D0%BE%D0%BA%D0%B0%D0%BC%D0%B8)  
   2К. [Перенаправление стандартного вывода команд](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#2%D0%BA-%D0%BF%D0%B5%D1%80%D0%B5%D0%BD%D0%B0%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5-%D1%81%D1%82%D0%B0%D0%BD%D0%B4%D0%B0%D1%80%D1%82%D0%BD%D0%BE%D0%B3%D0%BE-%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D0%B0-%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4-pipe)  
3. [ДАННЫЕ ДЛЯ ТРЕНИРОВКИ](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#3-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D0%B5-%D0%B4%D0%BB%D1%8F-%D1%82%D1%80%D0%B5%D0%BD%D0%B8%D1%80%D0%BE%D0%B2%D0%BA%D0%B8)
    * [Концентрация белков в пробах морской воды](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#-%D0%BA%D0%BE%D0%BD%D1%86%D0%B5%D0%BD%D1%82%D1%80%D0%B0%D1%86%D0%B8%D1%8F-%D0%B1%D0%B5%D0%BB%D0%BA%D0%BE%D0%B2-%D0%B2-%D0%BF%D1%80%D0%BE%D0%B1%D0%B0%D1%85-%D0%BC%D0%BE%D1%80%D1%81%D0%BA%D0%BE%D0%B9-%D0%B2%D0%BE%D0%B4%D1%8B)  
    * [Динамика изменений углекислого газа в зависимости от разнообразия тундровых растительных сообществ на Аляске и в Швеции (Shaver et al., 2007)](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#-%D0%B4%D0%B8%D0%BD%D0%B0%D0%BC%D0%B8%D0%BA%D0%B0-%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B9-%D1%83%D0%B3%D0%BB%D0%B5%D0%BA%D0%B8%D1%81%D0%BB%D0%BE%D0%B3%D0%BE-%D0%B3%D0%B0%D0%B7%D0%B0-%D0%B2-%D0%B7%D0%B0%D0%B2%D0%B8%D1%81%D0%B8%D0%BC%D0%BE%D1%81%D1%82%D0%B8-%D0%BE%D1%82-%D1%80%D0%B0%D0%B7%D0%BD%D0%BE%D0%BE%D0%B1%D1%80%D0%B0%D0%B7%D0%B8%D1%8F-%D1%82%D1%83%D0%BD%D0%B4%D1%80%D0%BE%D0%B2%D1%8B%D1%85-%D1%80%D0%B0%D1%81%D1%82%D0%B8%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D1%8B%D1%85-%D1%81%D0%BE%D0%BE%D0%B1%D1%89%D0%B5%D1%81%D1%82%D0%B2-%D0%BD%D0%B0-%D0%B0%D0%BB%D1%8F%D1%81%D0%BA%D0%B5-%D0%B8-%D0%B2-%D1%88%D0%B2%D0%B5%D1%86%D0%B8%D0%B8-shaver-et-al-2007)
    * [Нуклеотидные последовательности щетинкочелюстных (тип Chaetognatha)](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#-%D0%BD%D1%83%D0%BA%D0%BB%D0%B5%D0%BE%D1%82%D0%B8%D0%B4%D0%BD%D1%8B%D0%B5-%D0%BF%D0%BE%D1%81%D0%BB%D0%B5%D0%B4%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D0%BE%D1%81%D1%82%D0%B8-%D1%89%D0%B5%D1%82%D0%B8%D0%BD%D0%BA%D0%BE%D1%87%D0%B5%D0%BB%D1%8E%D1%81%D1%82%D0%BD%D1%8B%D1%85-%D1%82%D0%B8%D0%BF-chaetognatha)
   * [Файл со списком праймеров и их параметрами](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY01_P3_BASH.md#-%D1%84%D0%B0%D0%B9%D0%BB-%D1%81%D0%BE-%D1%81%D0%BF%D0%B8%D1%81%D0%BA%D0%BE%D0%BC-%D0%BF%D1%80%D0%B0%D0%B9%D0%BC%D0%B5%D1%80%D0%BE%D0%B2-%D0%B8-%D0%B8%D1%85-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D0%B0%D0%BC%D0%B8)  


### 1. Командная оболочка `BASH` (`B`ourne `A`gain `SH`ell)

<img src="https://bashlogo.com/img/logo/png/full_colored_dark.png" alt="BASH LOGO" width="360" border="5" />

#### 1A. Основные команды

| ФАЙЛЫ | НАВИГАЦИЯ | СИСТЕМА | УПРАВЛЕНИЕ |
| --------- | --------- | --------- | --------- |
| `touch` – создание файла | `mkdir` – создание пустой директории | `uname` – информация | `which` – путь к команде |
| `cat` – вывод строк файла | `rmdir` – удаление пустой директории | `hostname` – имя хоста | `chmod` – изменение прав |
| `less` и `more` – чтение файла | `ls` – список содержимого | `whoami` – имя пользователя | `chown` – изменение владельца |
| `nano`, `vim`, `emacs` – текстовые редакторы | `pwd` – путь к папке | `date` – дата и время | `env` – вывод переменных среды |
| `file` – тип файла | `cd` – перемещние между директориями | `cal` – календарная дата | `set` – управление средой BASH |
| `tr` – конвертация символов | `find` – поиск файлов по иерархии | `time` - время исполнения команды | `export` - добавление переменных в среду |
| `sed`, `awk` – текстовые процессоры | `mv` – перемещение/переименование | `who` – пользователи в системе | `apt-get` – установка программ |
| `tar`,`gzip` – архивация  | `cp` – копирование| `id` – инфа о пользователе | `ssh` – удаленное подключение |
| `diff` – сравнивает строки в двух файлах | `rm` – удаление | `df` – место на диске | `make` – компиляция |
| `head` – первые строки | `sleep` - гибернация | `fdisk` – разделы диска | `pkill` – остановка процесса |
| `tail` – конечные строки | `du` – размер директории | `ps` – активные процессы | `kill` – остановка программы |
| `wc` – счетчик | `wget` – скачивание | `lsof` – открытые файлы | `killall` – остановить все процессы |
| `grep` – поиск строк | `curl` – скачивание | `alias` – сокращения команд | `fg` – запуск процесса |
| `sort` – сортировка строк | `help` – справка | `clear` – очистка экрана | `bg` – запуск в фоновом режиме |
| `uniq` – уникальные строки (для сортированных данных) | `man` – помощь по команде | `top` – процессы в памяти | `echo` – вывод в консоль |
| `cut` –  разделение строк | `history` – история команд | `mount` – управление дисками | `ln` – создание ссылок |

#### 1Б. Специальные символы в `BASH` 
   `.` – рабочая директория  
   `..` – директория уровнем выше  
   `/` – корневой каталог или разделитель директорий в пути  
   `~` – домашняя директория  
   `#` – обозначение комментария  
   `$` – обозначение переменной  
   `&` – выполнение команды в фоновом режиме  
   `*` – символ подстановки  
   `(` – начало подзадачи  
   `)` – конец подзадачи  
   `\` – экранирование символов  
   `\\` – символ `\`  
   `|` – перенаправление стандартного вывода команды в стандартный ввод другой команды (конвейер)  
   `[` – символы подстановки  
   `]` – символы подстановки  
   `{` – обозначение блока команды  
   `}` – обозначение блока команды  
   `;` – разделитель команд  
   `'` – сильные кавычки  
   `"` – слабые кавычки  
   `<` – перенаправление стандартного ввода команды из файла  
   `>` – перенаправление стандартного вывода команды в новый файл  
   `>>` – добавление стандартного вывода команды в файл  
   `?` – символ подстановки  
   `!` – отрицательное условие (логическое отрицание)  
   `||` – логическая операция ИЛИ  
   `&&` - логическая операция И (также возможна при выполнении последовательности команд)  
   `:` – пустая команда (условие TRUE)  

#### 1В. Управление командной строкой `BASH` путем нажатия клавиш
   `TAB` – автозавершение команды или пути  
   `Ctr+L` – очистка экрана  
   `Ctr+S` – пауза (заморозка)  
   `Ctr+Q` – запуск (после паузы)  
   `Ctr+С` – экстренная остановка программы (`Ctr+\` – усиленная остановка)  
   `Ctr+Z` – заморозка программы 
   `Ctr+A` – перемещение в начало строки  
   `Ctr+E` – перемещение в конец строки  
   `Ctr+U` – удаление строки с начала до  
   `Ctr+K` – удаление строки с до конца 
   `Ctr+D` – конец ввода 
   `Ctr+F` ИЛИ `ВПРАВО` – перемещение вперед на один символ  
   `Ctr+B` ИЛИ `ВЛЕВО`– перемещение назад на один символ  
   `Ctr+W` – удаление последнего слова  
   `Ctr+T` – поменять местами две соседние буквы  
   `Ctr+P` ИЛИ `ВВЕРХ` – предыдущая команда в истории  
   `Ctr+N` ИЛИ `ВНИЗ` – следующая команда в истории  

#### 1Г. Переменные среды `BASH`(избранные):
   `$HOME` – путь к домашней директории  
   `$USER` – имя пользователя  
   `$PATH` – путь запуска программ  
   `$SHELL` – имя консоли

#### 1Д. Символы подстановки (wildcards)
   `?` - шаблон заменяющий ровно один символ  
   `*` – шаблон заменяющий любую последовательность символов, начиная с нулевой  
   `+` - последовательность из одного и более символов  
   `[]` - шаблон заменяющий любой из перечисленных в скобках символов  
   `{}` – задание диапазона или перечня символов для шаблона 

### 2. УПРАЖНЕНИЯ

##### 2А. Вывод строк и значений переменных на экран
```
echo HELLO WORLD!
echo $USER					# ПОКАЗЫВАЕТ ИМЯ ПОЛЬЗОВАТЕЛЯ
whoami					# ТОЖЕ ПОКАЗЫВАЕТ ИМЯ ПОЛЬЗОВАТЕЛЯ

#**********************************************************************#
### САМОСТОЯТЕЛЬНО ВЫВЕДИТЕ НА ЭКРАН ВАШЕ ИМЯ
```

##### 2Б. Перемещение и операции с директориями
```
pwd				# ПУТЬ К РАБОЧЕЙ (ТЕКУЩЕЙ) ДИРЕКТОРИИ
echo $HOME			# ПУТь К ДОМАШНЕЙ ДИРЕКТОРИИ

ls				# ПРОСМОТР СОДЕРЖИМОГО ДИРЕКТОРИИ
mkdir CLASS			# СОЗДАНИЕ НОВОЙ ДИРЕКТОРИИ
ls
cd CLASS			# ПЕРЕМЕЩЕНИЕ В ДИРЕКТОРИЮ CLASS
pwd
ls
#**********************************************************************#
cd ~				# ПЕРЕМЕЩЕНИЕ В ДОМАШНЮЮ ДИРЕКТОРИЮ
ls
cd /				# ПЕРЕМЕЩЕНИЕ В КОРНЕВУЮ ДИРЕКТОРИЮ
ls
cd				# ПЕРЕМЕЩЕНИЕ В ДОМАШНЮЮ ДИРЕКТОРИЮ
ls
cd ~/Desktop			# ПЕРЕМЕЩЕНИЕ В ДИРЕКТОРИЮ РАБОЧЕГО СТОЛА
ls
cd ~/Downloads			# ПЕРЕМЕЩЕНИЕ В ДИРЕКТОРИЮ DOWNLOADS
ls
cd -				# ПЕРЕМЕЩЕНИЕ В ПРЕДЫДУЩУЮ ДИРЕКТОРИЮ
#**********************************************************************#
### САМОСТОЯТЕЛЬНО ПЕРЕМЕСТИТЕСЬ В ДИРЕКТОРИЮ CLASS И ПРОВЕРЬТЕ ЕЕ СОДЕРЖИМОЕ
cd .				# РАБОЧАЯ (ТЕКУЩАЯ) ДИРЕКТОРИЯ
cd ..				# ПЕРЕМЕЩЕНИЕ В ДИРЕКТОРИЮ УРОВНЕМ ВЫШЕ
pwd
ls
```

##### 2В. Просмотр истории команд
```
history
### пролистывание предущих команд возможно клавишами ВВЕРХ и ВНИЗ
### умное дописывание команд возможно с помощью клавиши TAB
### перемещение в начало командной строки CTR+A
### перемещение в конец командной строки CTR+E
### удаление командной строки от положения курсора в сторону ее начала Ctr+U
### удаление командной строки от положения курсора в сторону ее конца Ctr+K
```

##### 2Г. Создание и чтение файлов
```
### ПЕРЕМЕСТИТЕСЬ В ДИРЕКТОРИЮ CLASS
ls
touch test					# СОЗДАНИЕ ПУСТОГО ФАЙЛА
less test					# ПРОСМОТР ФАЙЛА (для выхода нажмите Q)
nano test					# РЕДАКТИРОВАНИЕ ФАЙЛА (выход CTR+X)
echo Hello world! > test 			# СОЗДАНИЕ НОВОГО ФАЙЛА, СОДЕРЖАЩЕГО СТРОКУ
less test
echo Check that! >> test 			# ЗАПИСЬ НОВОЙ СТРОКИ В СУЩЕСТВУЮЩИЙ ФАЙЛ
less test
#**********************************************************************#
cat test					# ВЫВОД ВСЕХ СТРОК ФАЙЛА
#**********************************************************************#
cp test test2					# КОПИРОВАНИЕ ФАЙЛА
ls
mv test2 test.txt				# ПЕРЕИМЕНОВАНИЕ ФАЙЛА
ls
less test.txt
mv test.txt ..					# ПЕРЕМЕЩЕНИЕ ФАЙЛА В ДИРЕКТОРИЮ НА УРОВЕНЬ ВЫШЕ
cd ..
ls
cp test.txt CLASS/newtest.txt		# КОПИРОВАНИЕ В ДРУГУЮ ДИРЕКТОРИЮ И ПЕРЕИМЕНОВАНИЕ ФАЙЛА
mv test.txt CLASS/oldtest.txt		# ПЕРЕМЕЩЕНИЕ В ДРУГУЮ ДИРЕКТОРИЮ И ПЕРЕИМЕНОВАНИЕ ФАЙЛА
#**********************************************************************#
cd CLASS
ls
cat newtest.txt oldtest.txt			# ВЫВОД СТРОК ДВУХ ФАЙЛОВ
#**********************************************************************#
### САМОСТОЯТЕЛЬНО СОХРАНИТЕ СОДЕРЖИМОЕ ФАЙЛОВ newtest.txt И oldtest.txt В ОДИН ФАЙЛ unified.dat
less unified.dat
```

##### 2Д. Символы подстановки (wildcards)
```
### ПЕРЕМЕСТИТЕСЬ В ДИРЕКТОРИЮ CLASS
ls
ls *.txt
ls test*
ls ???test.txt
ls test.[tx]??
cat *.txt					# ВЫВОД ВСЕХ СТРОК ФАЙЛОВ С РАСШИРЕНИЕМ txt
cat *.txt > unified.dat				# СОХРАНЕНИЕ СТРОК ВСЕХ ФАЙЛОВ С РАСШИРЕНИЕМ txt
### САМОСТОЯТЕЛЬНО ПРОВЕРЬТЕ СОДЕРЖИМОЕ ФАЙЛА unified.dat
### ЧТО ИЗМЕНИЛОСЬ?
```

##### 2E. Вызов справки (help и man)
```
help					# ВЫВОД ОБЩЕЙ СПРАВКИ BASH
help pwd				# ВЫВОД СПРАВКИ ПО СТАНДАРТНОЙ КОМАНДЕ
help -s pwd				# ВЫВОД СОКРАЩЕННОЙ ИНСТРУКЦИИ (аргумент -s)
man pwd					# ОТКРЫТИЕ ФАЙЛА С ПОДРОБНОЙ ИНСТРУКЦИЕЙ (для выхода нажмите Q)
man man
#**********************************************************************#
### ПЕРЕМЕСТИТЕСЬ В ДИРЕКТОРИЮ CLASS
### САМОСТОЯТЕЛЬНО ПРОВЕРЬТЕ ДЕЙСТВИЕ АРГУМЕНТОВ КОМАНДЫ ls, ПОЛЬЗУЯСЬ СПРАВКОЙ
ls -l
ls -a
ls -F
ls -s
ls -S
ls -al
ls -alr
ls -alh
```

##### 2Ë. Удаление папок и файлов
```
### ПЕРЕМЕСТИТЕСЬ В ДИРЕКТОРИЮ CLASS
ls
rm test						# УДАЛЕНИЕ ФАЙЛА test
ls
rm *.txt					# УДАЛЕНИЕ ФАЙЛОВ С РАСШИРЕНИЕМ *.txt
cd ..
rmdir CLASS					# НЕУДАЧНАЯ ПОПЫТКА УДАЛЕНИЯ ДИРЕКТОРИИ CLASS
cd -
ls 
rm *						# УДАЛЕНИЕ ВСЕХ ФАЙЛОВ В РАБОЧЕЙ ДИРЕКТОРИИ
cd ..
rmdir CLASS					# УСПЕШНАЯ ПОПЫТКА УДАЛЕНИЯ ДИРЕКТОРИИ CLASS
#**********************************************************************#
mkdir CLASS{1..3}				# СОЗДАНИЕ СРАЗУ НЕСКОЛЬКИХ ДИРЕКТОРИЙ
ls
rmdir CLASS?					# УДАЛЕНИЕ СРАЗУ НЕСКОЛЬКИХ ПУСТЫХ ДИРЕКТОРИЙ
ls
#**********************************************************************#
mkdir -p ./ONE/TWO/THREE			# СОЗДАНИЕ НЕСКОЛЬКИХ ВЛОЖЕННЫХ ДИРЕКТОРИЙ
ls
ls ONE
ls ONE/TWO
#**********************************************************************#
rmdir ONE					# НЕУДАЧНАЯ ПОПЫТКА УДАЛЕНИЯ ДИРЕКТОРИИ ONE
rm -r ONE					# ОПАСНОЕ УДАЛЕНИЕ НЕПУСТОЙ ДИРЕКТОРИИ ONE
ls
```

##### 2Ж. Подстановки команд и меры предосторожности для новичков
```
alias						# ПОКАЗЫВАЕТ СУЩЕСТВУЮЩИЕ ПОДСТАНОВКИ КОМАНД
alias cp='cp -i'				# ЗАЩИТА ПРОТИВ УДАЛЕНИЯ ФАЙЛА ПРИ КОПИРОВАНИИ
alias mv='mv -i'				# ЗАЩИТА ПРОТИВ УДАЛЕНИЯ ФАЙЛА ПРИ КОПИРОВАНИИ
set -o noclobber				# ЗАЩИТА ПРОТИВ УДАЛЕНИЯ ФАЙЛА ПРИ СОХРАНЕНИИ ПОТОКА (>)
#**********************************************************************#
### СОХРАНЕНИЕ МЕР БЕЗОПАСНОСТИ В НАСТРОЙКАХ КОНСОЛИ
less ~/.profile
echo alias cp='cp -i' >> ~/.profile
echo alias mv='mv -i' >> ~/.profile
echo set -o noclobber >> ~/.profile
```

##### 2З. Проверка типа консоли
```
echo $SHELL				# ВЫВОД НА ЭКРАН ПУТИ РАБОЧЕЙ КОНСОЛИ
cat /etc/shells				# ВЫВОД НА ЭКРАН СПИСКА ВСЕХ ДОСТУПНЫХ ДЛЯ ВЫБОРА КОНСОЛЕЙ
#**********************************************************************#
### ЕСЛИ У ВАС СЕЙЧАС ПО УМОЛЧАНИЮ СТОИТ НЕ BASH
### ТО ИСПОЛЬЗУЙТЕ КОМАНДУ chsh -s /bin/bash
### И ПЕРЕЗАПУСТИТЕ КОНСОЛЬ
```

##### 2И. Скачивание файлов из сети
```
### СОЗДАЙТЕ И ПЕРЕМЕСТИТЕСЬ В ДИРЕКТОРИЮ CLASS
### СКАЧИВАЕМ ФАЙЛ С ПОМОЩЬЮ КОМАНДЫ wget
#**********************************************************************#
wget https://raw.githubusercontent.com/vinni-bio/LEEBAO-BIOINFORMATICS/master/FILES/north-pacific-gyre/NENE01729B.txt
#**********************************************************************#
### ИЛИ ИСПОЛЬЗУЙТЕ CURL###
#**********************************************************************#
### СОХРАНЕНИЕ ФАЙЛА ПОД ЕГО ИМЕНЕМ
curl -O https://raw.githubusercontent.com/vinni-bio/LEEBAO-BIOINFORMATICS/master/FILES/north-pacific-gyre/NENE01729B.txt
#**********************************************************************#
### СОХРАНЕНИЕ ФАЙЛА ПОД ДРУГИМ ИМЕНЕМ
curl https://raw.githubusercontent.com/vinni-bio/LEEBAO-BIOINFORMATICS/master/FILES/north-pacific-gyre/NENE01729B.txt -o proba.txt
#**********************************************************************#
### ВЫВОД ИНФОРМАЦИИ И СОХРАНЕНИЕ В ФАЙЛ
curl https://raw.githubusercontent.com/vinni-bio/LEEBAO-BIOINFORMATICS/master/FILES/north-pacific-gyre/NENE01729B.txt 
#**********************************************************************#
curl https://raw.githubusercontent.com/vinni-bio/LEEBAO-BIOINFORMATICS/master/FILES/north-pacific-gyre/NENE01729B.txt > test.txt
#**********************************************************************#
### СВОДКА ИНФОРМАЦИИ ПО ФАЙЛУ
curl -I https://raw.githubusercontent.com/vinni-bio/LEEBAO-BIOINFORMATICS/master/FILES/north-pacific-gyre/NENE01729B.txt 
#**********************************************************************#
rm test.txt proba.txt
#**********************************************************************#
### ПОЛУЧЕНИЕ ДАННЫХ ИЗ ГЕННОГО БАНКА С ПОМОЩЬЮ КОМАНДЫ curl
curl -s 'https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgi?id=AF086833.2&db=nuccore&rettype=fasta'
```

##### 2Й. Работа с файловыми строками
```
cat NENE01729B.txt				# ВЫВОД ВСЕХ СТРОК
head NENE01729B.txt				# ВЫВОД ПЕРВЫХ 10 СТРОК
head -n2NENE01729B.txt				# ВЫВОД ПЕРВЫХ 2 СТРОК
tail -n2 NENE01729B.txt				# ВЫВОД ПОСЛЕДНИХ 5 СТРОК
tail -n +2 NENE01729B.txt			# ВЫВОД ВСЕХ СТРОК КРОМЕ ПЕРВОЙ
grep 22 NENE01729B.txt				# ПОИСК СТРОК ПО ПАТТЕРНУ
wc NENE01729B.txt				# СТАТИСТИКА ФАЙЛА
wc -l NENE01729B.txt				# КОЛИЧЕСТВО СТРОК
wc -w NENE01729B.txt				# КОЛИЧЕСТВО СЛОВ
wc -с NENE01729B.txt				# КОЛИЧЕСТВО БУКВ
sort NENE01729B.txt				# СОРТИРОВКА СТРОК
cut -d. -f1 NENE01729B.txt			# РАЗДЕЛЕНИЕ И ВЫВОД СТОЛБЦОВ
cut -d. -f1 NENE01729B.txt > test.txt
uniq test.txt
```

##### 2К. Перенаправление стандартного вывода команд (pipe)
```
cat NENE01729B.txt | head
cat NENE01729B.txt | wc -l
cat NENE01729B.txt | cut -d. -f1 | head
cat NENE01729B.txt | cut -d. -f1 | uniq
cat NENE01729B.txt | cut -d. -f1 | sort | uniq
cat NENE01729B.txt | cut -d. -f1 | sort | uniq | wc -l
```

### 3. ДАННЫЕ ДЛЯ ТРЕНИРОВКИ

#### • Концентрация белков в пробах морской воды

[ссылка на данные](https://github.com/vinni-bio/LEEBAO-BIOINFORMATICS/tree/master/FILES/north-pacific-gyre)

Нелли - морской биолог. Недавно она вернулась из шестимесячной научной экспедиции в северной части Тихого океана, где она собирала биологические образцы желеподобного вида в [Большом тихоокеанском мусорном пятне](https://ru.wikipedia.org/wiki/%D0%91%D0%BE%D0%BB%D1%8C%D1%88%D0%BE%D0%B5_%D1%82%D0%B8%D1%85%D0%BE%D0%BE%D0%BA%D0%B5%D0%B0%D0%BD%D1%81%D0%BA%D0%BE%D0%B5_%D0%BC%D1%83%D1%81%D0%BE%D1%80%D0%BD%D0%BE%D0%B5_%D0%BF%D1%8F%D1%82%D0%BD%D0%BE). Всего ей удалось собрать 1520 проб, которые она должна была прогнать через специальный прибор, измеряющий относительное содержание 300 белков в каждой пробе и сохраняющий данные каждого измерения в отдельный файл. Затем Нелли нужно было проанализировать полученные результаты (1520 файлов) в программе `goostats`. По завершении анализа она собиралась опубликовать полученные результаты в специальном номере журнала *Aquatic Biology*. Для этого ей нужно было отправить свой манускрипт до конца месяца.

Самое ужасное это то, что Нелли каждый раз нужно вручную загружать новый файл в программу `goostats`, чтобы проанализировать полученные данные. Получается, что она должна открывать эту программу 1520 раз, а затем ждать целую минуту покамест не закончится анализ данных, чтобы запустить следующий файл. Таким образом, Нелли понадобилось бы больше суток непрерывной работы. Однако, с помощью командной строки BASH, теперь Нелли может сделать эту работу гораздо быстрее и проще, автоматизировав все рутинные процессы, связанные с открытием и закрытием файлов, а также с запуском очередного анализа. Тем самым она смогла освободить себе время, чтобы сконцентрировать свое внимание на написании статьи, успев опубликовать ее в нужные сроки.

#### • Динамика изменений углекислого газа в зависимости от разнообразия тундровых растительных сообществ на Аляске и в Швеции (Shaver et al., 2007)

[ссылка на данные](https://raw.githubusercontent.com/vinni-bio/LEEBAO-BIOINFORMATICS/master/FILES/shaver_etal.csv)

Арктические ландшафты характеризуются экстремальной разобщенностью и различиями по растительному разнообразию. Эта разобщенность создает определенные затруднения для использования моделей, предсказывающих общую концентрацию углекислового газа и ее динамику в зависимости от изменений условий окружающей среды. Используемые нами для тренировки данные были собраны на Аляске и в Швеции для построения и тестирования новой модели динамики углекислового газа в тундровой зоне.

#### • Нуклеотидные последовательности щетинкочелюстных (тип Chaetognatha)

[ссылка на данные](https://github.com/vinni-bio/LEEBAO-BIOINFORMATICS/tree/master/FILES/Sequences)

Десять файлов формата FASTA interleaved. Каждый файл включает одну нуклеотидную последовательность.

#### • Файл со списком праймеров и их параметрами

[ссылка на данные](https://raw.githubusercontent.com/vinni-bio/LEEBAO-BIOINFORMATICS/master/FILES/primers.txt)

Включает набор из последовательностей 22 праймеров, созданных программой Primer3.
Обозначения столбцов:
1. Название праймера
2. Позиция первого нуклеотида праймера на референсном геноме
3. Длина последовательности праймера
4. Температура плавления праймера
5. Содержание GC в последовательности праймера
6. Устойчивость праймера к самогибридизации (чем меньше тем лучше)
7. Устойчивость 3' конца праймера к самогибридизации (чем меньше тем лучше)
8. Нуклеотидная последовательность праймера