В папке Backend содержится исходный код сервера, а также его собранные модули (в подпапке bin)
В паке Agetn содержится исходный код вычислителя (пока не готово)

Сервер запускается простым запуском Backend\bin\calculatorServer.exe, затем в браузере нужно открыть localhost:8081
Под Windows проект можно собрать запустив Backend\Build.bat

Структура проекта Backend:
cmd\calculatorServer - точка входа в приложение (функция main)
http\api - handler обрабатывающий обращения к серверу
internal\application\application.go - запуск и остановка сервера 