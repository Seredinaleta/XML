XML
 1. Создать внешний репозиторий c названием XML.
 Create repository XML

 2. Клонировать репозиторий XML на локальный компьютер.
 git clone https://github.com/Seredinaleta/XML

 3. Внутри локального XML создать файл “new.xml”.
 cd XML
 touch new.xml
 4. Добавить файл под гит.
 git add .

 5. Закоммитить файл.
 git commit -m"Xml file added"

 6. Отправить файл на внешний GitHub репозиторий.
git push

 7. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
vim new.xml
insert
<?xml version="1.1" encoding="utf-8"?>
<Name>
        <First_Name>Yuliia Trubina</First_Name>
        <Last_Name>Trubina</Last_Name>
</Name>
<Age>44</Age>
<Pets>1</Pets>
<Salary>2000</Salary>
cat new.xml
Esc :wq

 8. Отправить изменения на внешний репозиторий.
git commit -m"Modified new.xml"
git push

 9. Создать файл preferences.xml
touch preferences.xml

 10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.
vim preferences.xml
insert
<?xml version="1.1" encoding="utf-8"?>
<Preferences>
        <favorite film>Prada</favorite film>
        <favorite serial>Stargate Atlantis</favorite serial>
        <favorite dish>Meat</favorite dish>
        <favorite season>Spring</favorite season>
        <next desired country>Crete</next desired country>
</Preferences>
Esc :wq


 11. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML
cat>>skills.xml

<?xml version="1.1" encoding="utf-8"?>
<Skill1>Theory of testing</Skill1>
<Skill2>Basic JavaScript </Skill2>
<Skill3>Client-server architecture</Skll3>
<Skill4>HTTP request methods and responce codes</Skill4>
<Skill5>Structures JSON and XML</Skill5>
<Skill6>DevTools of web browsers</Skill6>
<Skill7>Mobile testing</Skill7>
<Skill8>Command line (Terminal)</Skill8>
<Skill9>SQL Basic</Skill9>
<Skill10>Scrum development methodology</Skill10>
<Skill11>API testing via Postman(JS,API autotests</Skill11>
CTRL Z


 12. Сделать коммит в одну строку.
 git add skills.xml preferences.xml|commit -m "Commit for 2 files at once"

 13. Отправить сразу 2 файла на внешний репозиторий.
git push

 14. На веб интерфейсе создать файл bug_report.xml.
Add file bug_report.xml

 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Commit new file

 16. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
<?xml version="1.0" encoding="utf-8"?>
<Bug_report>
 <Main> 
   <ID>number</ID>
   <Summary>Short text description jf the bug</Summary>
   <STR>Steps to reproduce the bug</STR>
   <ER>Estimated result of the test</ER>
   <AR>Actual result of the test</AR>
   <Severity>The degree of influence a defect has on the product's operation blocker/crititical/major/minor/trivial</Severity>
  </Main>
  <Additional>
    <Priority>The order in which the defect should be fixed ASAP/high/medium/low</Priority>
   <Environment>Conditions Device Type/OS/Browser/Software version/Connection Strength/Screen size/Zoom level/Pixel ratio etc</Environment>
    <Visual Proof>Screenshots, videos, text, logs of Bug</Visual Proof>
   </Additional>
  <Reporter_Name>Your own</Reporter_Name>
  <Status>SDLS status Opened/In Progress/Fixed or Ready for check/Reopened/Closed/Deffered/Rejected</Status>

 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Commit changes Update bug_report.xml

 18. Синхронизировать внешний и локальный репозиторий XML
git fetch
git pull

