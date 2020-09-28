# hello-world
it will show how to print hello world in python.
now i am making some changes.



1.  create a repositery in which u want to upload your project.
2. type in gitbash 'git init' ( inside your project folder which u want to upload)
3. then type 'git remote add origin https://github.com/kapilchhipa4/game-in-javascript.git' (it is the link of your repositery)
4.  git remote -v  ( check origin)
5. git add . ( it will add all the files of your folder)
6. git commit -m "some message"  ( commit the changes)
7. git  push -f origin master   ( now u can push on origin )
8 done;




make new branch and upload updated project------------

1.  type in gitbash 'git init' ( inside your project folder which u want to upload)
2. then type 'git remote add origin https://github.com/kapilchhipa4/game-in-javascript.git' (it is the link of your repositery)
3. git remote -v  ( check origin)
4. git checkout -b new-branch-name
5. git add . ( it will add all the files of your folder)
6. git commit -m "some message"  ( commit the changes)
7. git  push -f origin 'your branch name'   ( now u can push on origin )


how to select a particular branch

1. git checkout branch_name

-------------------------------------------------------------------------------------------
E: Could not get lock /var/lib/dpkg/lock - open (11: Resource temporarily unavailable)
E: Unable to lock the administration directory (/var/lib/dpkg/), is another process using it?

fix that error

1. ps aux | grep -i apt
2. kill process with 'kill process_id' command 

 2.1 sudo kill -9 <process_id>  ( to kill forcefully)
 
 2.2 sudo killall apt apt-get ( to kill all process)
 
 --------------------------------------------------------------------------------------------------
 how to edit a file
 sudo -i gedit /etc/apt/sources.list
