# Exam_2420

## Part 1

- run command ``` sudo apt update && sudo apt upgrade```


## Part 2

-  I  used the following keys to navigate the file
```
h = left, l = right, j = down and k = u
```

- I used ```x``` to delete each character need to replace the old one 
- Then used ```c``` to change to new character

![](images/1.png)

**NOTE** I forgot screenshot the ketbings ToT 

## Part 3

![](images/2.png)
![](images/3.png)
![](images/5.png)
![](images/6.png)

## Part 4

```
#!/bin/bash


echo "regular user on the system are:"

grep x:[0-5][0-9][0-9][0-9] -ri /etc/passwd

echo "Users currently logged in are: vargrant"

```

## Part 5
- put the service file to ```/etc/systemd/system```

- service file

```
[Unit]
Description=show all the users in vagrant also current login user

[Service]
Type=simple
Environment=DIR=/home/vagrant/final
ExecStart=/etc/systemd/system

[Install]
WantedBy=multi-user.target

```

![](images/8.png)

## Part 6

- Timer file
```
Unit]
Description=My Service Timer

[Timer]
# Run the timer 1 minute after booting
OnBootSec=1min
# Run the timer every day at the same time
OnUnitActiveSec=1d

[Install]
# Start the timer and the associated service when the timer is activated
WantedBy=multi-user.target

```

