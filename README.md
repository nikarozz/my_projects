# ussc_project
1. Before proceeding with the deployment of the website, you need to make sure that all available updates 
are installed on the existing linux ubuntu image, as well as docker and docker-compose.

2. Create a folder with any name, for example, "project", using the command:
$ mkdir project
We go into it using the command:
$ cd project 

3. Initialize an empty git repository in our folder:
$ git init

4. Connect to the repository on github using the command:
$ git remote add origin https://github.com/nikarozz/ussc_project

5. Download files from the repository:
$ git pull https://github.com/nikarozz/ussc_project master

6.Using the ls command, we check the contents of the project folder, now it should contain a yml-file, 
two folders and readme.md.
 
7. We raise our site in one command:
$ sudo docker-compose up -d

8. Check the connectivity:
$ curl localhost:8080/index.php 
 
9. If the machine for some reason cannot connect to github, then the files necessary for deployment should be manually moved to the project folder,
then steps 7 and 8 should be performed.
