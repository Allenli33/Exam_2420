# Exam_2420

## part 1

- run command ``` sudo apt update && sudo apt upgrade```


## part 2

-  I  used the following keys to navigate the file
```
h = left, l = right, j = down and k = u
```

- I used ```x``` to delete each character need to replace the old one 
- Then used ```c``` to change to new character

![](images/1.png)

## part 3

![](images/2.png)
![](images/3.png)
![](images/5.png)

## part 4

```
#!/bin/bash


echo "regular user on the system are:"

grep x:[0-5][0-9][0-9][0-9] -ri /etc/passwd

echo "Users currently logged in are: vargrant"

```

## part 5
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
