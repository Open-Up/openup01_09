# Practice scripting

## Question 1

Write a script reporting the twenty biggers file or directories inside a folder.

Your command should show size of the folder/file in human readeable form. It should contain then only the name of the directory. It should be sorted from bigger (top) to smaller (bottom).

It should list only files in the current directory.

Example of output : 

```
benwa@horizon ~/Music % ./script.sh
3,3G	./Red Hot Chili Peppers
2,2G	./antoine
1,3G	./Mes BOs
1,1G	./Nightwish
1,1G	./Boom Boom
929M	./Cypress Hill
918M	./Metallica
794M	./Guns N' Roses
782M	./Unknown Artist
704M	./muse
666M	./Rancid
631M	./Led Zeppelin
623M	./Pen of Chaos
606M	./D'espairsRay
600M	./Sonata Arctica
600M	./Pink Floyd
596M	./Rammstein
573M	./Time Machine
533M	./Nobuo Uematsu
530M	./The Police
```

Command seen : du, sort, tail, head, cut

## Question 2

**data_2.csv** is in the Coma Separated Value format. It has a header about what composes each line of the file.

Please propose scripts for : 

 - Counting number of lines

Exemple of output :

```
benwa@horizon ~/Documents/linagora/open-up/s01/e07 (git)-[master] % ./script.sh
10
```

Command seen : wc, tail, tr, cut

 - Sorting employees name (and only there name) by alphabetic order

Example of output : 

```
benwa@horizon ~/Documents/linagora/open-up/s01/e07 (git)-[master] % ./script.sh
Alfred
Cuong
Dung
Giap
Manford
Michael
Name
Quynhn
Robert
Sang
Tuan
```

Command seen : sort, cut, head

 - Sorting the employees by age

Example of output : 

```
benwa@horizon ~/Documents/linagora/open-up/s01/e07 (git)-[master] % ./script.sh
10 Manford
22 Cuong
24 Sang
25 Giap
26 Tuan
35 Michael
41 Dung
41 Quynhn
65 Alfred
75 Robert
```

Command seen : sort, cut, head

 - Returning the sum of there income

```
benwa@horizon ~/Documents/linagora/open-up/s01/e07 (git)-[master] % ./script.sh
5250
```

Command seen : awk

## Question 3 : Automation

 - Run every hour a report of top 10 folders in your home. Append results to ~/space.log
 - Add a report on boot. Append results to ~/space-start.log
 - Manage the log. rotate it every week. Keep 6 months. Compress it.
