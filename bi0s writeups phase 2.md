**Bandit writeups** 

**level0**- connected to the bandit in the terminal and used **the cat** command to get the password **level1**- used a password which I got in the previous level and I used **cat** command to get the  

`            `password 

**level2**- I used **ls** command for a list of files where the bandit password hides and used **cat** command  

` `to get the password for the next level 

**Level 3**- used **ls** command to list the files on the bandit website it said that the password is stored in  

`   `a hidden file but in the list the file is not there then I tried and got that the hidden file is  

`              `stored in the inhere directory. 

**level4**-  used **ls** command to list the files in the bandit website it said that the password is stored in an inhere directory in a readable format then I used **find** command to which file the format is and used **cat** command to get the password 

**level5**-  used **find** command to find the files with a given file size and used **cat** command to get the               password 

**level6**- used again find command to find the files with the given conditions and at last used **cat**  
**
`             `command 

**level7**- used **ls** and **find** and **grep -c** command to find the file with the given conditions 

`             `grep -c is used to count the no of files in txt format and gives us how many txt files are  

`             `there. 

**level8**- used **sort** and **uniq** commands to get the password 

`             `**sort** command used to keep all the txt files in alphabetical order and **uniq** command used to               delete all the repeated files. 

**level9**- used **strings** and **grep** command 

grep command is used to filter the content which makes us easy 

**level10**- used **ls** command and used base64 command 

`              `base64 is used to conevert an binary strings to txt format 

**level11**- used **cat** command and **tr** command. 

`               `tr command used to translate the characters 

**level12**- used **cp, xxd, zcat, bzcat, tar** commands to get the password 

`               `**cp** command is used to copy the files 

`                `**xxd** is used to create an hex dump file from a folder 

`    `**zcat** is used to view the contents without compressing an folder 

`    `**bzcat** is used to decompresses the files to an standard output 

`    `tar is used save several files into an archive file 

**level13**- used **ssh** command and get through the resources given in the website 

`               `**ssh** command used to provides a secured connection between two hosts over an insecure  

`               `network. 

**level14**- used **nc** command and used the google to proceed to next step and at last I got that how to                     do 

`              `**nc** command used to transfer data 

**level15**- used **openssl** command and referred to google to do this 

`              `at starting I don’t know how to do the task and I used google and chatgpt to do the task. 

`              `**Openssl** command is used to generate private keys. 

**Level16**- used **nmap** and vim commands in this level 

`                `at starting we have to use **nmap** command which scans the ip address and detect the   

`                `installed applications and vim command is used to navigate and edit the files easily. 

**Level 17**-  used **diff** commands in this level. According to the question, they said that only one line  

`               `has been changed so we have to use diff command. 

`              `**diff** command is used to compare two files. 

**level18**- We have to use **sshpass** command to do this task. At starting I tried this task by using  

`    `**ssh** command only but after that, I searched on Google and I found to know that we  

`               `have to use **sshpass** command. Then, we have to use **ls** command to see which files are 

`               `there and a readme file will be present. We have to use **cat** command to open this file for  

`               `the password. 

`               `**sshpass** command used for password authentication. 

**Level19-**  In this task when we see the list of files by using  **ls**  command there will be a **setuid**  

`                 `Binary file. Then we have to run this file as another user.  

`                 `**Setuid** allows users to run an executable with the file system permissions of 

`                 `the executable's owner or group respectively and to change behaviour in directories. 

**Level20-** To start this level I opened two bandit20 windows as explained in the first hint. The first   

`               `one will be used to run the setuid command and the second one will be to run the network[  ](https://en.wikipedia.org/wiki/Setuid)

`               `daemon. To start the network daemon we can use "nc" to receive the information coming                                in from the setuid script. The second part of the command sends the current password for  

`               `verification from the setuid script. Now that we are listening for a response, I used the  

`               `"./suconnect 1234" command to run the script and get the next password. After running the  

`               `script I received the confirmation that the password matches and that it sends the  

`               `password for the next level. 

**Level21-**  According to the given resource on the website there is a configuration for a cron job on  

`                `"/etc/cron.d/" to complete this level. First, we have to change the directory to 

`                `"/etc/cron.d/" and we have to see what files are present in this directory. So, for that, we   

`                `have to use the **ls** command to see the list of files. Once it shows the files we want only  

`                `the file where the password for level 22 is hidden. I used cat command to see what cron  

`                `job is doing it is executing a bash script at every minute of every hour as explained by the  

`                `stars in the beginning. 

**Level22-** This level is also the same as above like there is a cron job configuration. When I read this  

`                `The file I saw is another bash file running every minute. According to the file it saves 

`                `The user running the file to a variable. Then it runs **echo** command which sends the string   

`                `to the md5sum command. Then it saves the hash to a variable. Then next it copies the  

`                `password or next level to a folder when we open this folder we will get the password 

`                `for the next level. 

`                `**Echo** command is used to allow users to display lines of text or strings that are passed as                  Arguments. 

**Level23-** This level is somewhat hard to do. The starting part is the same as the previous level. 

`                `After moving into that directory and reading the folder, I see that the folder runs and  

`                `then deletes all of the scripts in that folder. Then I changed the directory to  

`                `"/var/spool/bandit24" and created a folder and ran some commands **#!/bin/bash** and  

`                `Read the file **/etc/bandit\_pass/bandit24*** save the file into a temporary folder.** After that  

`               `I saved the file and ran chmod command to adjust permissions so that anybody can  

`                `Execute it. Once it finishes running I read the temporary file using ls command to get the                  Password for next level. 

**Level24-** For this level, I created a script that runs a loop which creates all possible values of  

`                `4digit combination. I used an echo command to do this task. I also used brute force also                      This Task which guesses username and password to gain unauthorized access. 

`                `It gave me the password for the next level. 

**Level25-** This level is hard for me I tried it so many times but didn’t get it. At last, I searched in  

`                `Google How to do this level and I learned from it. We have to connect to the bandit26  

`                `Server and it will close automatically because it is not bin bash. The script shows **more**  
**
`                `On that file to show the ASCII text and then exits directly. The more command may be  

`               `The entry point that exploits the normal shell. So, we have to resize the terminal window. 

`               `To edit this file we have to use **v** command which edits the file. Next we have to enter the 

`               `Edited mode to check the password for next level. 

**Level26-** To do this level it is needed to get a shell for bandit26. Once we got the shell we can  

`               `Find the file in bandit26 home directory then we have to use **ls** command and it just  

`               `Runs a command as another user. Next we can print this file to get the password 

`               `For next level. 

**Level27-** In this level we will use **git clone** command to copy the github profile where the password                 For the next level is hidden. For this we have to create a temporary directory and then we                     Clone into it. Once we cloned the git profile we will use **ls** command and **cd** command  

`                `To find the password. 

**Level28-** This level is also same as the previous level but at last the password is hidden. 

`                 `Then we have to use some git commands to get the hidden password. So, we have to use 

`                 `**git log** to see there are any commits. Then the commit with missing data will be there. 

`                 `So, we use **git checkout** command to retrieve the data. Then we will get the password for 

`                  `Next level. 

**Level29-** This level is also as same as the previous level but at end at the password’s place it comes  

`                `As passwords in production so we use **gitlog** and **git branch** commands to get the  

`                `Password for the next level. 

`                `**git branch** command used to create, list, delete branches. 

**Level30-** This level also same as previous level but at the end it changes. At end we have to use  

`                `**git tag and git show** commands. 

`                `**git tag** command used to specify the important points in the repository 

`                `**git show** command used to expand the details in the git.             

**Bi0s writeups(Phase2)** 

**Ot security:** 

-I have gone through the resources given in the pdf. I referred through google and chatgpt for better understanding. 

-Still I have to read the resources once again to understand it better because it’s an new topic to me it takes time to understand.  

**Automotive:** 

-I have read the car hacking book but I didn’t understood it much better I have to read once again the book 

- the can utils task is very interesting. I have referred through the github profile to do the can utils task and I referred to chatgpt and youtube for doing this task.  

**Embedded:** 

-I have listened the arduino programming video and I have to work on it for better understanding because it needs C languagr so I know basics of C language still I have to work on it.  

- I have finished the first two tasks where I have referred to google and chatgpt for this task and it’s very interesting.  

-I didn’t done the last task. I have tried to do the task but I didn’t know how to start. So, after the interview I will do this task and learn the arduino programming once again.  

**Web:**  

I have learned html and css from the given resources.** 

I have completed the first task that is to create a portfolio and the first task in picoctf but I didn’t able to complete the remaining tasks 

**Firmware reversing:** 

I have watched the video about the intro to rev and assembly  

But I didn’t able to complete the remaining things because I have more interest on automotive and embedded Mainly the can-utils task is very  

Interesting to do. I have done it in the hardware ctf but I didn’t 

remember all the procedure to do this. So, again I learned about can-utils and commands to use I this task.   
