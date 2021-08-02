# JPAdemoExample
**Error:**
************************** APPLICATION FAILED TO START *************************** Description: Web server failed to start. Port 8080 was already in use. Action: Identify and stop the process that's listening on port 8080 or configure this application to listen on another port.

**Solution:**
Check what processes are running at available ports.
netstat -ao |find /i "listening"
OR
netstat -ano | find "8080" (Note: 8080 is port fail to start)

Taskkill /F /IM 6592 Note: Mention correct Process Id
C:\Users\HOME>Taskkill /F /IM 14664
SUCCESS: The process with PID 14664 has been terminated.


![image](https://user-images.githubusercontent.com/63113379/127901374-eb9986ad-6a60-4534-8630-fad4bbdb2555.png)
Process 15828 is running on port 8080.



DB:
login:http://localhost:8080/h2-console
![image](https://user-images.githubusercontent.com/63113379/127909710-bd3608ba-199e-4733-9c02-d1296b998b6e.png)

Data inserted from the form :

![image](https://user-images.githubusercontent.com/63113379/127909493-c1fd2cda-c988-4f7f-ac09-854be70900cc.png)
