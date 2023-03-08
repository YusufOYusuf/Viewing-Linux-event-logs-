<h1>Using Reconnaissance Tools</h1>


<h2>Description</h2>
In this lab, I learned to view event logs in Kali Linux. Log files are a set of records that Linux maintains for the administrators to keep track of important events.
<br />



<h2>Environments Used </h2>

- <b>Kali GNU/Linux Rolling</b> 

<h2>Utilities and Language </h2>

- <b>Terminal</b>

<h2>Program walk-through:</h2>

<p align="center">
Navigate to the Terminal window <br>
Enter the following commands <br>
"ls /var/log" (view the default system log directory/ older logs are periodically archived as .gz files) <br>
<img src="https://i.postimg.cc/HxN9p1Gm/Screen-Shot-2023-03-07-at-5-53-44-PM.png" height="80%" width="80%" alt=""/>
<br />

  
  
<p align="center">
Enter the following commands <br>
"sudo cat /var/log/syslog" (allows you to view the syslog file) <br>
<img src="https://i.postimg.cc/fRBNB8nX/Screen-Shot-2023-03-07-at-5-57-27-PM.png" height="80%" width="80%" alt=""/>
<br />



<p align="center">
Enter the following commands <br>
"sudo tail /var/log/syslog" (allows you to view the last 10 lines of a file) <br>
<img src="https://i.postimg.cc/cLY33tVV/Screen-Shot-2023-03-07-at-5-59-37-PM.png" height="80%" width="80%" alt=""/>
<br />




<p align="center">
Enter the following commands <br>
"sudo grep “CRON” /var/log/syslog " (allows you to display all lines of syslog with the word CRON) <br>
<img src="https://i.postimg.cc/KznFrxZc/Screen-Shot-2023-03-07-at-6-02-47-PM.png" height="80%" width="80%" alt=""/>
<br />





<p align="center">
Open a new Terminal window <br>
Enter the following commands <br>
"sudo tail -f -n 5 /var/log/auth.log " (-f allows you to monitor a log file i real time/ -n allows you to input how many lines you want) <br>
<img src="https://i.postimg.cc/6QnkdfKJ/Screen-Shot-2023-03-07-at-6-08-20-PM.png" height="80%" width="80%" alt=""/>
<br />






<p align="center">
Return to the first terminal window <br>
Enter the following commands <br>
"sudo head -n 50 /var/log/auth.log | tail" (By piping the output of head you'll view lines 41-50 of auth.log) <br>
If you navigate back to the 1st window you will notice the last command appears in auth.log. sudo invokes privileged operations <br>
<img src="https://i.postimg.cc/RV0QKCmv/Screen-Shot-2023-03-07-at-6-16-07-PM.png" height="80%" width="80%" alt=""/>
<br />


















