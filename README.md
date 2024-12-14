Automatically-Keep-Mobile-Hotspot-Alive-Windows 10/11
#Source

https://superuser.com/a/1434648

https://gist.github.com/primaryobjects/8b54f7f4219960127f1f620116315a37


Right on the windows start button and on click the "Event Viewer" or Search bar and type "Event Viewer"

![1](https://github.com/user-attachments/assets/2b8e2c41-5e2e-4e60-b5b6-53e9fcd0fa06)
![2](https://github.com/user-attachments/assets/5c987ebb-405a-4498-abe8-fcf284292282)

# Event Viewer Step

Click on "Applications and Serices Logs" then "Microsoft" then "Windows" find "NetworkProfile" and "WLAN-AutoConfig"

NetworkProfile is for your internet 
WLAN-AutoConfig is for your hotspot

**Event ID you need the know:**
 
Event ID 10000 is for NetworkProfile

Event ID 8008 is for WLAN-AutoConfig

# Task Scheduler Step

Click Search bar and type "Task Scheduler" and the click "Create Task" name it "Automatic Hotspot" give the task a description "Turn on the hotspot when you have internet connection" next
set the "Configure for" to Windows 10 or Windows 11  turn on "Run with highest privileges" and "Hidden"

Click the Triggers tab

Click on "New" to make a trigger

Set "Begin the task" On an event

Next follow the picture this trigger is for turn on the hotspot when you connect to the wifi

![3](https://github.com/user-attachments/assets/861ccf06-216a-42ae-b915-682154f53859)


and this trigger is for turn on the hotspot if it turn off 

![4](https://github.com/user-attachments/assets/52745e6b-462f-489e-b9a0-deee31219368)

Click Actions tab

Click on "New" to make a actions 

Set "Program/script" to the file patch for the cmd code you downloaded


Click Constions tab

Next follow the picture

![5](https://github.com/user-attachments/assets/e224075e-28f0-441e-9e5f-415abcf69abb)


Click Setting tab 

set it up to your needs 




