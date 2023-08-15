# **Linux terminal (GitBash) commands №1**

1. Посмотреть где я - `pwd`
2. Создать папку - `mkdir foldername`
3. Зайти в папку - `cd foldername`
4. Создать 3 папки - `mkdir foldername1 foldername2 foldername3`
5. Зайти в любоую папку - `сd foldername1`
6. Создать 5 файлов (3 txt, 2 json) - `touch touch 1.txt 2.txt 3.txt 4.json 5.json`
7. Создать 3 папки - `mkdir foldername4 foldername5 foldername6`
8. Вывести список содержимого папки - `ls -la`
9. Открыть любой txt файл - `vim 1.txt`
10. + написать туда что-нибудь, любой текст. `i`
11. + сохранить и выйти. `esc :wq `
12. Выйти из папки на уровень выше `cd ..`
13. переместить любые 2 файла, которые вы создали, в любую другую папку. `mv foldername1/3.txt foldername2/3.txt  mv foldername1/4.json foldername2/4.json`
14. скопировать любые 2 файла, которые вы создали, в любую другую папку. `cp foldername1/1.txt foldername2/1.txt   cp foldername1/2.txt foldername3/2.txt`
15. Найти файл по имени `find . -name "1.txt"`
16. просмотреть содержимое в реальном времени (команда grep) изучите как она работает. `tail -F foldername1/1.txt`
17. вывести несколько первых строк из текстового файла `head -n3 foldername1/1.txt`
18. вывести несколько последних строк из текстового файла `tail -n4 foldername1/1.txt`
19. просмотреть содержимое длинного файла (команда less) изучите как она работает. `less foldername1/1.txt`-->  ` q `
20. вывести дату и время `date`
_______________________________________________________________________________________________________________________________________
Задание *
1. Отправить http запрос на сервер.http://162.55.220.72:5006/terminal-hw-request  
`curl "http://162.55.220.72:5006/terminal-hw-request"`

2. Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
<pre>`nano`

cd foldername
mkdir foldername1 foldername2 foldername3
cd foldername1
touch 1.txt 2.txt 3.txt 4.json 5.json
mkdir foldername4 foldername5 foldername6
ls -la
cd ..
mv foldername1/3.txt foldername2/3.txt
mv foldername1/4.json foldername2/4.json</pre>

`Ctrl+X далее Y далее script.sh`

Запуск 
<pre>./script.sh`
total 4
drwxr-xr-x 1 Елена 197121 0 Aug  4 18:52 .
drwxr-xr-x 1 Елена 197121 0 Aug  4 18:52 ..
-rw-r--r-- 1 Елена 197121 0 Aug  4 18:52 1.txt
-rw-r--r-- 1 Елена 197121 0 Aug  4 18:52 2.txt
-rw-r--r-- 1 Елена 197121 0 Aug  4 18:52 3.txt
-rw-r--r-- 1 Елена 197121 0 Aug  4 18:52 4.json
-rw-r--r-- 1 Елена 197121 0 Aug  4 18:52 5.json
drwxr-xr-x 1 Елена 197121 0 Aug  4 18:52 foldername4
drwxr-xr-x 1 Елена 197121 0 Aug  4 18:52 foldername5
drwxr-xr-x 1 Елена 197121 0 Aug  4 18:52 foldername6</pre>




