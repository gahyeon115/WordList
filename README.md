start /b cmd /c "node index.js"
timeout /t 5 /nobreak > nul
start http://localhost:3000
이 3개의 코드를 가지고 있는 test.bat 배치파일이 소스코드 zip 에 존재합니다. 
각각의 코드에 대한 설명은 아래와 같습니다. 
start /b cmd /c "node index.js" -> index.js 파일을 실행하여 서버를 백그라운드에서 시작합니다.
timeout /t 5 /nobreak > nul -> 서버가 안정적으로 시작될 시간을 주기 위해 5초 동안 대기하는 명령어입니다.
5초 대기 후, start http://localhost:3000 명령을 통해 기본 웹 브라우저를 열리면,  http://localhost:3000 페이지가 표시됩니다.

이 과정을 통해 압축된 소스파일에 존재하는 test.bat 파일을 더블클릭하여 실행하게 되면 웹페이지를 확인할 수 있습니니다.





