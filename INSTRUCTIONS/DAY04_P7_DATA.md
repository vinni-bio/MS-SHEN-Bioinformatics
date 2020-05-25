# LEEBAO-BIOINFORMATICS

Интенсивный курс по биоинформатике для магистрантов ШЕН

## ДЕНЬ 03. ПРАКТИКА: ВЫРАВНИВАНИЕ ПОСЛЕДОВАТЕЛЬНОСТЕЙ И АНАЛИЗ ЭВОЛЮЦИОННОЙ МОДЕЛИ

## СОДЕРЖАНИЕ

1. [НЕОБХОДИМЫЕ ПРОГРАММЫ](https://github.com/vinni-bio/MS-SHEN-Bioinformatics/blob/master/INSTRUCTIONS/DAY03_P7_DATA.md#1-%D0%BD%D0%B5%D0%BE%D0%B1%D1%85%D0%BE%D0%B4%D0%B8%D0%BC%D1%8B%D0%B5-%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D1%8B)



### 1. НЕОБХОДИМЫЕ ПРОГРАММЫ
* Текстовый редактор [SUBLIME TEXT 3](https://www.sublimetext.com/3) ИЛИ [Notepad++](https://notepad-plus-plus.org/downloads/) (только Windows)
* [MEGA X](http://www.megasoftware.net/)
* [Sequence Matrix](http://gaurav.github.io/taxondna/)

### A. Проверьте количество записей в Генном банке по исследуемой группе (например, медведи):
1. Зайдите на страницу Генного банка `http://www.ncbi.nlm.nih.gov`
2. Найдите кнопку **All Resources**  в левом меню
3. В списке баз данных выберите **Nucleotide Database**
4. В поисковой строке введите запрос и нажмите кнопку поиска **SEARCH**:
`all[filter]`
5. В левом меню найдите фильтр **_Species_** и нажмите кнопку **customize**
6. Добавьте исследуемую группу (`Ursidae`) и нажмите кнопку **add**
7. Сколько записей относится к исследуемой группе?

### Б. Загрузите на свой компьютер записи исследуемой группы для анализа:
1. Зайдите снова в Генный банк (**Nucleotide Database**)
2. В поисковой строке введите запрос `"Yu L"[AUTH] AND Ursidae[ORGN] AND irbp[TITL]`
3. Сохраните последовательности в формате 'FASTA':<br/>
[irbp-ursidae.fasta](https://raw.githubusercontent.com/vinni-bio/WS-20160909/master/LAB1/irbp-ursidae.fasta)
4. В поисковой строке введите запрос `mitochondrion[filter] AND Ursidae[ORGN] AND "Talbot SL"[AUTH] AND 1140[SLEN]`
5. Сохраните последовательности в формате 'FASTA':<br/>
[cytb-ursidae.fasta](https://raw.githubusercontent.com/vinni-bio/WS-20160909/master/LAB1/cytb-ursidae.fasta)

### В. Выбор внешней группы
1. Откройте вкладку **Resources** в верхнем меню
2. Выберите **Sequence Analysis** и нажмите **_BLAST (Basic Local Alignment Search Tool)_**
3. Выберите <img src="https://blast.ncbi.nlm.nih.gov/images/nucleutide-blast-cover.png" 
alt="Nucleotide BLAST" width="360" border="5" />
4. Введите номер NCBI для анализа последовательности вида *Ursus maritimus*:`AY303843.1`
5. Выберите базу данных **Nucleotide collection** и исключите медведей `Ursidae` из поиска
6. Нажмите <img src="https://blast.ncbi.nlm.nih.gov/images/blastButtonDown.jpg" 
alt="BLAST" width="360" border="5" />
7. Просмотрите результаты поиска и выберите наиболее подходящую последовательность со 100% покрытием:
`Panthera pardus` [AY525041.1](https://www.ncbi.nlm.nih.gov/nuccore/AY525041.1) (Леопард)
8. Сохраните внешнюю группу по гену *irbp* в отдельный файл в формате 'FASTA':<br/>
[irbp-outgroup.fasta](https://raw.githubusercontent.com/vinni-bio/WS-20160909/master/LAB1/irbp-outgroup.fasta)
9. Зайдите снова в Генный банк (**Nucleotide Database**)
10. В поисковой строке введите запрос `mitochondrion[filter] AND "Panthera pardus"[ORGN] AND "complete genome"[TITL]`
11. Выберите любой полный митохондриальный геном вида *Panthera pardus* (например, [KP001507.1](https://www.ncbi.nlm.nih.gov/nuccore/KP001507.1))
12. Выберите  **Change region shown** в правом меню и укажите координаты от `15000` до `16500`. Нажмите кнопку **update**.
13. Сохраните внешнюю группу по гену *cytb* в отдельный файл в формате 'FASTA':<br/>
[cytb-outgroup.fasta](https://raw.githubusercontent.com/vinni-bio/WS-20160909/master/LAB1/cytb-outgroup.fasta)

