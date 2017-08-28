# Setting up a linux-server

For this Udacity-project, I configured a linux-server. I used Amazon Lightsail as a server instance. In the end, my Citydatabase-Webapp is running on the server.



### IP-address & URL
The static public IP of the server is 52.28.203.240, the private IP is 172.26.6.48.
The URL of the server is http://ec2-52-28-203-240.eu-central-1.compute.amazonaws.com.



### Summary of installed software
For getting the server running, I installed the following software:
1. apache2
2. libapache2-mod-wsgi
3. postgresql & postgresql-contrib
4. python-requests
5. python3-sqlalchemy
6. python-sqlalchemy
7. python-oauth2client
8. python-pip
9. virtualenv



### Summary of steps
1. Creating new user "grader" and giving him sudo-rights
2. Generating a Key Pair with ssh-keygen for the grader-user, storing the private key on my local machine.
3. Checking the file /etc/ssh/sshd_config if connecting with password is disabled.
4. In sshd_config, disable the remote access for root.
4. Changing in the same file the port for ssh-check-in from 22 to 2200.
5. Preparing the firewall, open the ports for NTC, the port 2200, closing port 22.
6. restarting ssh-service
7. Installing apache2 & mod_wsgi
8. Writing the wsgi-file
9. Preparing my flask-directory-structure and my project-python-files.
10. Renaming my project.py-file to __init__.py
11. Configure a new virtual host
12. restarting Apache
13. installing postgresql on server
14. creating new role for postgresql
15. creating new database
16. creating new linux-user with same name as new postgresql-role
17. starting my database setup with catalogdb.py
18. populating database with catalogpopulate.py
19. Changing url in the google developer console for logging in with google.



### Used third party software
This project uses Python, Flask and Bootstrap.