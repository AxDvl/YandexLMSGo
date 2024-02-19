В папке Backend содержится исходный код сервера, а также его собранные модули (в подпапке bin). 
В паке Agent содержится исходный код вычислителя

Сервер запускается простым запуском Backend\bin\calculatorServer.exe, затем в браузере нужно открыть localhost:8081. 
Агент запускается запуском Agent\bin\Agent.exe  (агентов можно запускать сколько угодно)
Под Windows проекты можно собрать запустив Backend\Build.bat и Agent\Build.bat. 

Структура проекта Backend:
 - cmd\calculatorServer - точка входа в приложение (функция main);
 - http\api - handler обрабатывающий обращения к серверу;
 - internal\application\application.go - запуск и остановка сервера;
 
Сохранение результатов в БД или на диск не реализовано