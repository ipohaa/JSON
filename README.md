Домашнее задание на тему GitHub
Работа с файловой системой Git, ознакомление с JSON  
+ [1. Создать внешний репозиторий c названием JSON](https://github.com/ipohaa/JSON#1-создать-внешний-репозиторий-c-названием-json)
+ [2. Клонировать репозиторий JSON на локальный компьютер](https://github.com/ipohaa/JSON#2-клонировать-репозиторий-json-на-локальный-компьютер)
+ [3. Внутри локального JSON создать файл "new.json"](https://github.com/ipohaa/JSON#3-внутри-локального-json-создать-файл-newjson)
+ [4. Добавить файл под гит](https://github.com/ipohaa/JSON#4-добавить-файл-под-гит)
+ [5. Закоммитить файл](https://github.com/ipohaa/JSON#5-закоммитить-файл)
+ [6. Отправить файл на внешний GitHub репозиторий](https://github.com/ipohaa/JSON#6-отправить-файл-на-внешний-github-репозиторий)
+ [7. Отредактировать содержание файла "new.json"](https://github.com/ipohaa/JSON#7-отредактировать-содержание-файла-newjson)
+ [8. Отправить изменения на внешний репозиторий](https://github.com/ipohaa/JSON#8-отправить-изменения-на-внешний-репозиторий)
+ [9. Создать файл preferences.json](https://github.com/ipohaa/JSON#9-создать-файл-preferencesjson)
+ [10. В файл preferences.json добавить информацию о своих предпочтениях в формате JSON](https://github.com/ipohaa/JSON#10-в-файл-preferencesjson-добавить-информацию-о-своих-предпочтениях-в-формате-json)
+ [11. Создать файл skills.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON](https://github.com/ipohaa/JSON#11-создать-файл-skillsjson-добавить-информацию-о-скиллах-которые-будут-изучены-на-курсе-в-формате-json)
+ [12. Отправить сразу 2 файла на внешний репозиторий](https://github.com/ipohaa/JSON#12-отправить-сразу-2-файла-на-внешний-репозиторий)
+ [13-14. На веб интерфейсе создать файл bug_report.json и сделать commit](https://github.com/ipohaa/JSON#13-14-на-веб-интерфейсе-создать-файл-bug_reportjson-и-сделать-commit-сохранить)
+ [15-16. На веб интерфейсе модифицировать файл bug_report.json и сделать commit](https://github.com/ipohaa/JSON#15-16-на-веб-интерфейсе-модифицировать-файл-bug_reportjson-добавить-баг-репорт-в-формате-json-и-сделать-commit-сохранить)
+ [17. Синхронизировать внешний и локальный репозиторий JSON](https://github.com/ipohaa/JSON#17-синхронизировать-внешний-и-локальный-репозиторий-json)

## 1. Создать внешний репозиторий c названием JSON.
+ Зайти и авторизоваться на сайте
+ Нажать `New repositories`
+ Ввести имя нового репозитория в поле `Repository name`
+ Нажать `Create repository`

## 2. Клонировать репозиторий JSON на локальный компьютер.
```
Ipohaa@MainPC MINGW64 /f/git
$ git clone https://github.com/<имя>/JSON.git
```
## 3. Внутри локального JSON создать файл "new.json".
```
Ipohaa@MainPC MINGW64 /f/git/JSON (main)
$ cat > new.json
```
## 4. Добавить файл под гит.
Так как мы создали новый файл и гит о нём не знает, его нужно индексировать, воспользуемся `git add <файл>` чтобы добавить новый файл
```
Ipohaa@MainPC MINGW64 /f/git/JSON (main)
$ git add new.json
```
## 5. Закоммитить файл. 
Синтаксис коммита `git commit -m "Описание коммита"`
```
$ git commit -m "Add new file new.json"
```
## 6. Отправить файл на внешний GitHub репозиторий.
```
$ git push
```
## 7. Отредактировать содержание файла "new.json"
Написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата) в формате JSON.
```
Ipohaa@MainPC MINGW64 /f/git/JSON (main)
$ vi new.json
```
## 8. Отправить изменения на внешний репозиторий.
Закоммитим наши изменения
```
$ git commit -am "Update file new.json"
```
и отправим на внешний репозиторий
```
$ git push
```
## 9. Создать файл preferences.json
```
Ipohaa@MainPC MINGW64 /f/git/JSON (main)
$ cat > preferences.json
```
## 10. В файл preferences.json добавить информацию о своих предпочтениях в формате JSON.
```
Ipohaa@MainPC MINGW64 /f/git/JSON (main)
$ vi preferences.json
```
## 11. Создать файл skills.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
```
Ipohaa@MainPC MINGW64 /f/git/JSON (main)
$ cat > skills.json
```
## 12. Отправить сразу 2 файла на внешний репозиторий.
Закоммитим наши изменения
```
$ git commit -m "Add new file preferences.json and skills.json"
```
и отправим на внешний репозиторий
```
$ git push
```
## 13-14. На веб интерфейсе создать файл bug_report.json и сделать commit (сохранить).
+ Создадим новый файл `Add file` -> `Create new file`
+ Назовём файл bug_report.json
+ Сохраним файл, выберем `Commit new file`
## 15-16. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON и сделать commit (сохранить).
Чтобы редактировать файл, нам нужно его выбрать, нажав на его имя в списке
+ Выбираем файл bug_report.json
+ Выбираем пиктограмму карандаша `Edit this file`
+ Редактируем в нужном для нас формате
+ Сохраняем -> `Commit changes`

## 16. Синхронизировать внешний и локальный репозиторий JSON
Воспользуемся `git pull` для того чтобы синхронизировать файлы из внешнего репозитория на локальном компьютере
```
Ipohaa@MainPC MINGW64 /f/git/JSON (main)
$ git pull
```
