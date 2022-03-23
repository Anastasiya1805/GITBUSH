<div align="center">

### ***"Команды TERMINAL LINUX"*** 
</div>

+ Посмотреть где я: `pwd`
+ Создать папку: `mkdir document_case`
+ Зайти в папку: `cd document_case`
+ Создать 3 папки: `mkdir Mir_1 Mir_2 Mir_3` 
+ Зайти в любоую папку: `cd Mir_1`
+ Создать 5 файлов (3 txt, 2 json): `touch crem_1.txt crem_2.txt crem_3.txt pirog_1.json pirog_2.json`
+ Создать 3 папки: `mkdir sok_1 sok_2 sok_3`
+ Вывести список содержимого папки: `ls -la`
+ Открыть любой txt файл:  `vim crem_1.txt`
+ Hаписать туда что-нибудь, любой текст: Для Windows нажать `i`, напишем: 
  
```The History of the English Language.
The Scariest Day of the Year
The Vikings were the people of the northern part of Europe
The Vikings made their attacks very quickly and without any warning
The Vikings travelled across a large area
```


+ Сохранить и выйти: выйти из режима редактирования клавишей esc, далее снизу слева ввести: `:wq` (сохранить и выйти). Нажать `enter`.
+  Выйти из папки на уровень выше: `cd ..`
+  Переместить любые 2 файла, которые вы создали, в любую другую папку:   `mv Mir_1/crem_2.txt Mir_1/crem_3.txt Mir_2`.
+  Cкопировать любые 2 файла, которые вы создали, в любую другую папку: `cp Mir_1/crem_1.txt Mir_3/crem_1.txt
cp Mir_1/pirog_1.json Mir_3/pirog_1.json`.
+ Найти файл по имени:  find -name crem_1.txt
+ просмотреть содержимое в реальном времени (команда grep) изучите как она работает: `tail -f crem_1.txt | grep '.*'`
+ Вывести несколько первых строк из текстового файла:  `head -n crem_1.txt`.
+ Вывести несколько последних строк из текстового файла:  `tail -n 3 crem_1.txt`.
+ Просмотреть содержимое длинного файла (команда less) изучите как она работает: `less Mir_1/crem_1.txt`.
+ Вывести дату и время: `date`.

<div align="center">

### ***"Дополнительное задание"*** 
</div>

+ Отправить http запрос на сервер.

+ `http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000`
 Отправить http запрос на сервер.
+ `http://162.55.220.72:5005/terminal-hw-request`

+ `curl -X GET "http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000"`

+ `curl -X GET "http://162.55.220.72:5005/terminal-hw-request"`

 
+ 2 Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13:
  
  `#!/bin/bash`

:heavy_check_mark: cd script

:heavy_check_mark: mkdir f_1 f_2 f_3

:heavy_check_mark: cd f_1

:heavy_check_mark: touch test_1.txt test_2.txt test_3.txt test_4.json test_5.json

:heavy_check_mark: mkdir f_1 f_2 f_3

:heavy_check_mark: ls -la

:heavy_check_mark: mv *.txt* f_1 & mv *.json* f_2

:heavy_check_mark: ls -la
+ `chmod +x good.sh`
+ `+ ./good.sh1`