# -IOT-week-5-tasks
**Task 4: Control robot movement using a website**
In this task we have made a website with buttons to control the robot, either move forward/backward or turn right/left
![image](https://user-images.githubusercontent.com/108147030/187029365-e9747878-b85b-4868-a539-2cca64637a10.png)

The way this work, we made a new table name "movement" in the database and the ESP32 code **Movement.ino**
in **Task4** will read the data from the database frequently using GET method. <br>
when the user click the forward button, the website will send "forward" to the database and ESP32 will read it to move forward, and when the user click the right button, we will send "right" to the database and ESP32 will also turn right. <br>
![image](https://user-images.githubusercontent.com/108147030/187029370-f19c4472-5700-48f5-8e0e-7b32c81cbfed.png)

As you see in the image above, we also register how long did the user pressed the button, he clicked the forward button for **3.3** seconds and clicked the right button for **1.6** seconds. This is useful later if we want the robot replay what the user clickd before.
