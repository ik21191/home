Manually  kill Tomcat Process from Command line
Go to (Open) Command Prompt (Press Window + R then type cmd Run this).
Run following commands to get all listening ports (If tomcat runnig on other ports apart from 8080)

netstat -aon | find /i "listening"

Apply port filter If you know port number


netstat -aon |find /i "listening" |find "8080"

As in below screen you will get PID and then  run the following command to kill the process

3 Copy PID from result set


taskkill /F /PID

Ex: taskkill /F /PID 13332
