Репозиторий для домашнего задания по терминалу Linux  
Курс Вадима Ксезндзова  
Группа 27
## Linux terminal (GitBash) commands1 ##
1. Посмотреть где я  
> pwd  
2. Создать папку  
> mkdir /c/qaz_1  
3. Зайти в папку  
> cd qaz_1  
4. Создать 3 папки
> mkdir qaz_2 qaz_3 qaz_4  
5. Зайти в любоую папку  
> сd qaz_2
6. Создать 5 файлов (3 txt, 2 json)  
> touch qa_1.txt qa_2.txt qa_3.txt qa1.json qa2.json  
7. Создать 3 папки  
> mkdir f1 f2 f3
8. Вывести список содержимого папки  
> ls -Rla  
> Рекурсивное отображение вложенных файлов, длинный листинг, отображение скрытых файлов  
9. Открыть любой txt файл  
> vim qa_1.txt  
10. Написать туда что-нибудь, любой текст  
> qwerty1 qwerty2 qwerty3 qwerty4 qwerty4 qwerty5 qwerty6  
11. Cохранить и выйти
> ESC :wq  
12. Выйти из папки на уровень выше  
> cd ..  
13. Переместить любые 2 файла, которые вы создали, в любую другую папку  
> mv qaz_2/{qa_1.txt,qa1.json} qaz_3/  
14. Cкопировать любые 2 файла, которые вы создали, в любую другую папку  
> cp qaz_2/{qa_2.txt,qa2.json} qaz_3/  
15. Найти файл по имени  
> find . -name qa_2.txt  
16. Просмотреть содержимое в реальном времени  
> tail -f qa_1.txt 
17. Вывести несколько первых строк из текстового файла  
> head -n 2 qa_1.txt  
> выведет первые 2 строчки из указанного файла, по умолчанию выводит первые 10 строк   
18. Вывести несколько последних строк из текстового файла  
> tail -3 qa_1.txt  
> выведет последние 3 строчки из указанного файла, по умолчанию выводит последние 10 строк    
19. Просмотреть содержимое длинного файла (команда less)  
> less qa_3.txt  
20. Вывести дату и время  
> date  
  
Задание *  
1. Отправить http запрос на сервер  http://162.55.220.72:5005/terminal-hw-request    
> Шаг 1 - curl "http://162.55.220.72:5005/terminal-hw-request"  
> Шаг 2 - curl "http://162.55.220.72:5005/get_method?name=Julia&age=38"  
2. Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13  
- создать файл myscript.sh  
> #1/bin/bash  
> cd qaz_1  
> mkdir qaz_2 qaz_3 qaz_4  
> сd qaz_2  
> touch qa_1.txt qa_2.txt qa_3.txt qa1.json qa2.json  
> mkdir f1 f2 f3  
> ls -la  
> mv qa_1.txt,qa1.json ../qaz_3  
- сделать файл исполняемым  
> chmod +x ./myscript.sh  
- запустить файл  
> ./myscript.sh  
  
     

   

  
