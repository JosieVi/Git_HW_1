# JSON
GIT Homework 1. JSON

 Проверить синтаксиc  файла JSON: https://jsoneditoronline.org/
 1. Создать внешний репозиторий c названием JSON.
 Выполняю действия на сайте: New repository -> JSON, ставлю галочку "Добавить Readme file", чтобы при клонировании на локальный компьютер не было предупреждения о клонировании пустой папки.

 2. Клонировать репозиторий JSON на локальный компьютер.
 $ git clone https://github.com/JosieVi/JSON.git

 3. Внутри локального JSON создать файл “new.json”.
 $ cd JSON 
 $ touch new.json

 4. Добавить файл под гит.
 $ git add new.json

 5. Закоммитить файл.
 $ git commit -m "add new.json to repository GIT_HW_1"

 6. Отправить файл на внешний GitHub репозиторий.
 $ git push

 7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
 $ nano new.json
{
  "Name": "Olga",
  "Age": 36,
  "Number of pets": 0,
  "Desired salary": "3000$"
}
Ctrl+C
Ctrl+X

 8. Отправить изменения на внешний репозиторий.
 $ git add . 
 $ git commit -m "add completed file new.json to repository JSON"
 $ git push
 
 9. Создать файл preferences.json
 $ touch preferences.json

 10. В файл preferences.json добавить информацию о своих предпочтениях (любимый фильм, любимый сериал, любимая еда, любимое время года, страна, которую хотели бы посетить)
 в формате JSON.
 $ nano preferences.json
{
  "Favorite movie": "Lord of the Rings",
  "Favorite TV show": "Queen's Gambit",
  "Favorite food": "Fruits",
  "Favorite time of year": "Spring",
  "Desired country": "Finland"
}
Ctrl+C
Ctrl+X

 11. Создать файл skills.json, добавить информацию о скиллах, которые будут изучены на курсе в формате JSON
 $ cat > skills.json
{
  "Skills": [
    "Linux terminal commands",
    "JavaScript",
    "Git",
    "Postman",
    "DBeaver"
  ]
}
Ctrl+C

 12. Отправить сразу 2 файла на внешний репозиторий.
 $ git add . 
 $ git commit -m "add files preferences.json, skills.json to repository JSON"
 $ git push
 
 13. На веб интерфейсе создать файл bug_report.json.
 Repository JSON -> Add file -> Create new file -> bug_report.json

 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 Commit new file

 15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
{
  "Bug #": 1,
  "Summary": "Login: Error messages in the login from are displayed in English",
  "Environment": "All browsers / devices",
  "Severity": "Major",
  "Steps for reproduce": [
    "1. Open https://",
    "2. Follow 'Inloggen' link",
    "3. Fill required fields with invalid data",
    "4. Click 'Inloggen' button",
    "5. Pay attention to error messages"
  ],
  "Actual results": "Error messages in the login form are displayed in English",
  "Expected results": "Error messages in the login form are displayed in the chosen language"
}
 
 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Commit changes

 17. Синхронизировать внешний и локальный репозиторий JSON
 $ git pull
