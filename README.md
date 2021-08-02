# JPAdemoExample


Check what processes are running at available ports.
netstat -ao |find /i "listening"
OR
netstat -ano | find "8080" (Note: 8080 is port fail to start)

Taskkill /F /IM 6592 Note: Mention correct Process Id
C:\Users\HOME>Taskkill /F /IM 14664
SUCCESS: The process with PID 14664 has been terminated.
