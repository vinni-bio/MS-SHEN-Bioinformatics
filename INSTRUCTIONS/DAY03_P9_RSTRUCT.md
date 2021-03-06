# LEEBAO-BIOINFORMATICS

Интенсивный курс по биоинформатике для магистрантов ШЕН


## ДЕНЬ 03. ПРАКТИКА: ТИПЫ ДАННЫХ И МЕТОДЫ РАБОТЫ С НИМИ В R


### 1. Векторы (vectors)

##### Способы создания численных векторов
```
A <- c(1,2,3,4,5,6,7,8,9,10)			# КОНКАТЕНАЦИЯ ЧИСЕЛ
B <- 11:20					# ДИАПАЗОН ЦЕЛЫХ ЧИСЕЛ
FRAC <- c(0.1,0.5,10.3,14.0)			# ВЕКТОР ДРОБНЫХ ЧИСЕЛ

A.seq <- seq(from=1,to=10,by=1)			# последовательность с заданным шагом
B.seq <- seq(from=11,to=20,length=10)		# последовательность с заданной длиной
C.seq <- sample(1:100,size=10,replace=TRUE)	# произвольная последовательность с заменой
D.seq <- rep(1,10)				# повторные числа
E.seq <- numeric()				# создание пустого вектора реальных чисел
F.seq <- numeric(3)				# создание вектора реальных чисел с 3 элементами
G.seq <- double()				# создание пустого вектора реальных чисел двойной точности
H.seq <- integer()				# создание пустого вектора целых чисел
I.seq <- raw()					# создание пустого байтового вектора
```

##### Алгебраические операции с численными векторами
```
A.seq + D.seq					# СУММА ВЕКТОРОВ
B.seq - A.seq					# ВЫЧИТАНИЕ ВЕКТОРОВ
B.seq + 2					# СКАЛЯРНОЕ СЛОЖЕНИЕ
B.seq - 2					# СКАЛЯРНОЕ ВЫЧИТАНИЕ
A.seq * B.seq					# ПРОИЗВЕДЕНИЕ ВЕКТОРОВ
A.seq * 2					# СКАЛЯРНОЕ ПРОИЗВЕДЕНИЕ
B.seq / A.seq					# ДЕЛЕНИЕ ВЕКТОРОВ
B.seq / 2					# СКАЛЯРНОЕ ДЕЛЕНИЕ
B.seq ^ A.seq					# ВОЗВЕДЕНИЕ ВЕКТОРОВ
A.seq ^ 5					# СКАЛЯРНОЕ ВОЗВЕДЕНИЕ
```

##### Алгебраические функции с численными векторами
```
sum(A)						# сумма всех элементов вектора
prod(A)						# произведение всех элементов
sqrt(A)						# квадратный корень элементов вектора
log(A)						# натуральный логарифм элементов вектора
log10(A)					# десятичный логарифм элементов вектора
exp(A)						# экспонента элементов вектора
max(A)						# элемент с наибольшим значением
min(A)						# элемент с наименьшим значением
range(A)					# элементы с минимальным и максимальным значениями
sort(A)						# сортировка элементов вектора по возрастанию
round(A,2)					# округление элементов вектора до 2го знака
rev(A) 						# обратный вектор
```

##### Операции с элементами вектора. Индексация элементов объекта в R начинается с 1
```
A.seq[1]				# ПЕРВЫЙ ЭЛЕМЕНТ ВЕКТОРА
A.seq[length(A.seq)]			# ПОСЛЕДНИЙ ЭЛЕМЕНТ ВЕКТОРА
A.seq[-1]				# ВЕКТОР БЕЗ ПЕРВОГО ЭЛЕМЕНТА
A.seq[-length(A.seq)]			# ВЕКТОР БЕЗ ПОСЛЕДНЕГО ЭЛЕМЕНТА
A.seq[c(2,3)]				# СУБВЕКТОР С 2м и 3м ЭЛЕМЕНТАМИ
A.seq[c(F,T,T,F,F,F,F,F,F,F)]		# СУБВЕКТОР С 2м и 3м ЭЛЕМЕНТАМИ
A.seq[c(2,1,4,7,3,5,6,10,8,9)]		# ИЗМЕНЕНИЕ ПОРЯДКА ЭЛЕМЕНТОВ В ВЕКТОРЕ
A.seq[1:length(A.seq)%%2==0]		# ЧЕТНЫЕ ЭЛЕМЕНТЫ ВЕКТОРА
A.seq[1:length(A.seq)%%2!=0]		# НЕЧЕТНЫЕ ЭЛЕМЕНТЫ ВЕКТОРА
A.seq[3] <- 5				# ЗАМЕНА 3го ЭЛЕМЕНТА ВЕКТОРА
A.seq[с(1,2,3)] <- c(3,2,1)		# ЗАМЕНА ПЕРВЫХ ТРЕХ ЭЛЕМЕНТОВ ВЕКТОРА
```

##### Конкатенация векторов
```
C.seq <- c(A.seq,B.seq)			# КОНКАТЕНАЦИЯ ВЕКТОРОВ A и B
C.seq <- append(A.seq,B.seq)		# КОНКАТЕНАЦИЯ ВЕКТОРОВ A и B
C.seq <- append(A.seq,B.seq, after=2)	# ВСТАВКА ВЕКТОРА A в B
```

##### Способы создания символьных векторов
```
A <- c("Masha", "Petya", "Lena", "Slava")	# КОНКАТЕНАЦИЯ СЛОВ
LETTERS						# ЗАГЛАВНЫЕ БУКВЫ
letters						# ПРОПИСНЫЕ БУКВЫ
month.abb					# МЕСЯЦЫ СОКРАЩЕННЫЕ
month.name					# МЕСЯЦЫ ПОЛНЫЕ
B <- LETTERS[1:5]				# ДИАПАЗОН ЗАГЛАВНЫХ БУКВ
b <- letters[1:5]				# ДИАПАЗОН ПРОПИСНЫХ БУКВ
С.seq <- sample(c("Masha", "Petya", 		# ПРОИЗВОЛЬНЫЙ НАБОР ИМЕН
	"Lena", "Slava"),10,replace=TRUE)
D.seq <- sample(LETTERS,10,replace=TRUE)	# ПРОИЗВОЛЬНЫЙ НАБОР БУКВ
E.seq <- rep("Masha",10)			# ПОВТОРНЫЕ СЛОВА
```

##### Создание вектора (универсальный способ)
```
A.vec <- vector(mode="numeric")			# ЧИСЛОВОЙ
B.vec <- vector(mode="integer")			# ЦЕЛЬНОЧИСЛЕННЫЙ
С.vec <- vector(mode="logical")			# ЛОГИЧЕСКИЙ
D.vec <- vector(mode="character")		# СИМВОЛЬНЫЙ
E.vec <- vector(mode="raw")			# ПРОСТОЙ
```

##### Логические векторы (logical)
```
A.bool <- c(TRUE,TRUE,FALSE,FALSE)
B.bool <- c(F,F,T,T)
A.seq>5
```

### 2. Факторные векторы (factors)

##### Способы создания факторных векторов
```
gender <- c("Female", "Male", "Female", "Female", "Male", "Male", "Male", "Female","Male", "Female" )
fac.gen <- factor(gender)				# СОЗДАНИЕ ФАКТОРНОГО ВЕКТОРА
levels(fac.gen)						# ПРОВЕРЯЕМ УРОВНИ ФАКТОРОВ
fac.gen <- factor(gender, levels=c("Male","Female","unknown"))
fac.gen <- factor(gender, levels=c("Male","Female","unknown"), labels=c(1,2,0))
fac.gen <- factor(gender, levels=c("Male","Female","unknown"), labels=c(1,2,0), ordered=TRUE)
droplevels(fac.gen)					# НЕ ПОКАЗЫВАТЬ НЕИСПОЛЬЗУЕМЫЕ УРОВНИ
summary(fac.gen)					# СВОДКА ЧАСТОТ ПО УРОВНЯМ
table(fac.gen)						# ТАБЛИЦА ЧАСТОТ
```

### 3. Матрицы (matrix)

##### Способы создания матриц
```
A.mat <- cbind(A.seq,B.seq)			# ОБЪЕДИНЕНИЕ ВЕКТОРОВ ПО КОЛОНКАМ
B.mat <- rbind(A.seq,B.seq)			# ОБЪЕДИНЕНИЕ ВЕКТОРОВ ПО РЯДАМ
C.mat <- matrix(sample(1:10,size=20, replace=TRUE), nrow=10, ncol=2, byrow=FALSE)
```

##### Информация о матрице
```
dim(A.mat)					# РАЗМЕРНОСТЬ МАТРИЦЫ
nrow(A.mat)					# ЧИСЛО РЯДОВ
ncol(A.mat)					# ЧИСЛО СТОЛБЦОВ
rownames(A.mat)					# НАИМЕНОВАНИЯ РЯДОВ
colnames(A.mat)					# НАИМЕНОВАНИЯ СТОЛБЦОВ
dimnames(A.mat)					# НАЗВАНИЯ ИЗМЕРЕНИЙ (list)
A.mat[3:4,1]					# значения 3й и 4й строки 1го столбца
```

##### Операции с матрицами
```
A.mat %*% B.mat				# ПЕРЕМНОЖЕНИЕ МАТРИЦ
t(A.mat)				# ТРАНСПОНИРОВАНИЕ МАТРИЦЫ
A.mat + t(B.mat)			# ПОПАРНОЕ СЛОЖЕНИЕ 
t(B.mat) - A.mat			# ПОПАРНОЕ ВЫЧИТАНИЕ
A.mat * t(B.mat)			# ПОПАРНОЕ УМНОЖЕНИЕ 
t(B.mat) / A.mat			# ПОПАРНОЕ ДЕЛЕНИЕ 
C.mat <- diag(5)			# СОЗДАНИЕ ДИАГОНАЛЬНОЙ МАТРИЦЫ
C.mat + 5 				# СКАЛЯРНОЕ СЛОЖЕНИЕ МАТРИЦЫ
C.mat - 5 				# СКАЛЯРНОЕ ВЫЧИТАНИЕ МАТРИЦЫ
C.mat * 5 				# СКАЛЯРНОЕ УМНОЖЕНИЕ МАТРИЦЫ
C.mat / 5 				# СКАЛЯРНОЕ ДЕЛЕНИЕ МАТРИЦЫ
eigen(A.mat)				# СОБСТВЕННОЕ ЗНАЧЕНИЕ И ВЕКТОР
```

### 4. Таблицы (data.frame)

##### Способы создания таблиц
```
dat1 <- data.frame(B=B.seq,C=C.seq)
dat2 <- as.data.frame(A.mat)
names(dat1) <- c("A","B")		# ИЗМЕНЕНИЕ ЗАГОЛОВКОВ СТОЛБЦОВ
rownames(dat1) <- letters[1:10]		# ИЗМЕНЕНИЕ ЗАГОЛОВКОВ СТРОК
```

##### Индексация столбцов и строк таблицы
```
dat1["A"]				# СТОЛБЕЦ "А"
dat1[,"A"]				# СТОЛБЕЦ "А"
dat1[1]					# СТОЛБЕЦ "А"
dat1[,1]				# СТОЛБЕЦ "А"
dat1[-2]				# СТОЛБЕЦ "А"
dat1[1,]				# СТРОКА "а"
dat1["a",]				# СТРОКА "а"
dat1["a","A"]				# ЗНАЧЕНИЕ СТОЛБЦА "А" и СТРОКИ "а"
dat1[1,1]				# ЗНАЧЕНИЕ СТОЛБЦА "А" и СТРОКИ "а"
```

##### Операции с таблицей
```
dat1$C <- LETTERS[1:10]				# ДОБАВЛЕНИЕ НОВОГО СТОЛБЦА
dat2 <- cbind(dat1,D=letters[11:20])		# СОЗДАНИЕ НОВОЙ ТАБЛИЦЫ ИЗ СТАРОЙ
subset(dat1,subset=A>15,select=c(B,C)) 		# ФИЛЬТРАЦИЯ СТОЛБЦОВ "В" и "С" ПО СТОЛБЦУ "А"
dat1 <- dat1[,names(dat1)!="C"]			# УДАЛЕНИЕ СТОЛБЦА "С"
dat2 <- dat2[,-2]				# УДАЛЕНИЕ СТОЛБЦА "B"
dat3 <- merge(dat1,dat2)			# СЛИЯНИЕ ТАБЛИЦ
merge(dat1,dat2,by="A")				# СЛИЯНИЕ ТАБЛИЦ ЧЕРЕЗ КОЛОНКУ "A"
edit(dat1)					# РЕДАКТИРОВАНИЕ ТАБЛИЦЫ ВРУЧНУЮ В TEMP ПЕРЕМЕННУЮ
fix(dat1)					# РЕДАКТИРОВАНИЕ ТАБЛИЦЫ ВРУЧНУЮ
dat3[order(dat3$B),]				# СОРТИРОВКА ТАБЛИЦЫ ПО СТОЛБЦУ "В"
```

##### Создание пустой таблицы со столбцами заданного типа
```
df <- data.frame(name=character(),
                   age=numeric(),
                   sex=factor(levels=c("M","F")),
                   stringsAsFactors = FALSE)
```


### 5. Списки (list)

##### Создание и конвертация списков
```
A.list <- list(A=1:10,B=1:100,C=LETTERS,E=dat3)
B.list <- list(5, 10, 15, 20, 25)
B.vec <- unlist(B.list)
```

##### Индексация списков
```
A.list$A					# ВЫЗОВ РАЗДЕЛА 'A' СПИСКА A.list
A.list['B']					# ВЫЗОВ РАЗДЕЛА 'B' СПИСКА A.list
A.list[2]					# ВЫЗОВ РАЗДЕЛА 'B' СПИСКА A.list
A.list[['B']]					# ВЫЗОВ СОДЕРЖИМОГО РАЗДЕЛА 'B' СПИСКА A.list
A.list[[2]]					# ВЫЗОВ СОДЕРЖИМОГО РАЗДЕЛА 'B' СПИСКА A.list
A.list[["E"]]$A					# ВЫЗОВ СОДЕРЖИМОГО СТОЛБЦА 'A' В ТАБЛИЦЕ РАЗДЕЛА 'D' СПИСКА A.list
A.list[[4]]$A					# ВЫЗОВ СОДЕРЖИМОГО СТОЛБЦА 'A' В ТАБЛИЦЕ РАЗДЕЛА 'D' СПИСКА A.list
A.list[[4]][[1]]				# ВЫЗОВ СОДЕРЖИМОГО СТОЛБЦА 'A' В ТАБЛИЦЕ РАЗДЕЛА 'D' СПИСКА A.list
A.list[[4]]$A[2]				# ВЫЗОВ ВТОРОГО ЭЛЕМЕНТА СТОЛБЦА 'A' В ТАБЛИЦЕ РАЗДЕЛА 'D' СПИСКА A.list
A.list[[4]][[1]][2]				# ВЫЗОВ ВТОРОГО ЭЛЕМЕНТА СТОЛБЦА 'A' В ТАБЛИЦЕ РАЗДЕЛА 'D' СПИСКА A.list
str(A.list)					# ПРОСМОТР ЭЛЕМЕНТОВ СПИСКА
```

##### Добавление, замена, слияние и удаление элементов списка
```
A.list$E <- 'PROBA'				# ДОБАВЛЕНИЕ ТЕКСТОВОГО ВЕКТОРА
A.list["E"] <- 'PROBA2'				# ЗАМЕНА ЭЛЕМЕНТА СПИСКА
A.list <- append(A.list,letters[1:5])		# ДОБАВЛЕНИЕ СРАЗУ НЕСКОЛЬКИХ ЭЛЕМЕНТОВ
A.list <- append(A.list,list(letters[1:5]))	# ДОБАВЛЕНИЕ НОВОГО ВЕКТОРА
A.list['A'] <- NULL 				# УДАЛЕНИЕ ЭЛЕМЕНТА 'A'
A.list[4:8] <- NULL 				# УДАЛЕНИЕ C 4 ПО 8 ЭЛЕМЕНТОВ
B.list <- c(A.list,list(A=1:10))		# СЛИЯНИЕ ДВУХ СПИСКОВ
```
