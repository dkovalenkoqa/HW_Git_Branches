GitHub. HW_2

1. На локальном репозитории сделать ветки для:
    - Postman

      > git branch Postman
    - Jmeter
      > git branch Jmeter
    - CheckLists
      > git branch CheckLists
    - Bug Reports
      > git branch BugReports
    - SQL
      > git branch SQL
    - Charles
      > git branch Charles
    - Mobile testing
      > git branch MobileTesting

2. Запушить все ветки на внешний репозиторий
     > git push --set-upstream origin SQL Postman MobileTesting Jmeter CheckLists Charles BugReports
3. В ветке BugReports сделать текстовый документ со структурой баг репорта
     > git checkout BugReports

     > nano bug_report.txt
     ```
      Bug_Name : Application crashes upon clicking the SAVE button while creating a new user.
      Bug ID : (It will be automatically created by the BUG Tracking tool once you save this bug).
      Area Path : USERS menu -> New Users
      Build Number : Version Number 5.0.1
      Severity : HIGH (High/Medium/Low) or 1
      Priority : HIGH (High/Medium/Low) or 1
      Assigned to : Developer-X
      Reported By : Your Name
      Reported On : Date
      Reason : Defect
      Status : New/Open/Active (Depends on the Tool you are using)
      Environment : "Windows 2003/SQL Server 2005
     ```
4. Запушить структуру багрепорта на внешний репозиторий
     > git add .

     > git commit -m "create bug_report.txt"

     > git push
5. Вмержить ветку BugReports в Main
     > git checkout main

     > git merge BugReports
6. Запушить main на внешний репозиторий.
     > git push
7. В ветке CheckLists набросать структуру чек листа.
     > git checkout CheckLists
     ```
      1. General information (for example, a link and log in details to the website).
      2. Name of the section (subsection).
      3. List of checks (with the required level of detail)ю
      4. Type of verification (positive, negative).
      5. Test data.
      6. The expected behavior of the system.
      7. Information about the test environment: device, browser, screen resolution, etc.
      8. Check result (passed, failed, not executed).
      9. Bug number or a link to it in Jira (if the test is not passed).
     ```
8. Запушить структуру на внешний репозиторий.
     > git add .

     > git commit -m "create check_list.txt"

     > git push
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
10. Синхронизировать Внешнюю и Локальную ветки Main
     > git checkout main
     
     > git pull
