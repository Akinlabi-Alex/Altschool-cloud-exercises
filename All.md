# ANSWERS TO ALTSCHOOL CLOUD EXERCISES PROJECT
## Exercise 1

     This content contains vagrantfile with private network set to dhcp and also the output after running ifconfig

## Exercise 2

    LINUX COMMANDS

     1. cal:This displays the calendar
     2. export -p:This shows a list of all currently exported environment variables.
     3. printenv:Displays the values of all evironment variables.
     4. who:This shows who is currently logged in.
     5. uname:This displays system information.
     6. last:This shows the recent login history of users.
     7. finger:This shows information about all the users currently logged into the system,including their usernames, login time and terminal.
     8. last reboot:This shows reboot history
     9. df:This displays free disk space
    10. w:This shows which users are online and what they are doing

## Exercise 3

     To create 3 groups – admin, support & engineering: 

         - sudo groupadd admin
         - sudo groupadd support
         - sudo groupadd engineering

     To  add the admin group to sudoers:

         - sudo visudo -f /etc/sudoers.d/admin   
       
     To create a user in each of the groups:
       
         - sudo useradd -m alex_admin -G admin
         - sudo useradd -m alex_support -G support
         - sudo useradd -m alex_engineering -G engineering

     To generate SSH keys for the user in the admin group:

         - sudo -u alex_admin ssh-keygen -t rsa
         - sudo su -alex _admin 

## Exercise 4
     To install PHP 7.4 on your local linux machine using the ppa:ondrej/php package repo:

         - sudo apt install software-proprties-common 
         - sudo add-apt-repository ppa:ondrej/php
         - sudo apt update 

     To check the version of PHP installed on your system:

         - php -v

     To view the content:
         - cat /etc/apt/sources.list 

## Exercise 5    
     You already have Github account, setup a GitLab account if you don’t have one already
     You already have a altschool-cloud-exercises project,

     To clone the project to your local system:

         -git clone <repository name>
     
     To setup your name and email in Git’s global config:     
       
         -git config --global user.name "Akinlabi Alexander".
         -git config --global user.emai"alexmiracle100gmail.com".

       Run the following commands:
         - git config -l; to displays the Git configuration settings for the current user.
         - git remote -v; is used to display the URLs of the remote repositories that your local repository is connected to. It has two URL. One is for fetching and the other is for pushing.
         - git log; this command is used to display the commit history of the current branch. It shows a list of commits, starting with the most recent one.
