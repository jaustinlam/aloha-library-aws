# Aloha Library
A fictional library built that allows user sign up, see books and check books in and out. Hosted on AWS.

## Installation
1. Download the Private key supplied seperately and save under a file id_rsa
2. Move the file to your local .ssh folder
3. Log in to the server by running "ssh -v grader@35.160.130.147 -p2200" in terminal. 
4. To access website files enter 'cd /var/www/catalog/catalog'
5. To make sudo edits you must be supplied a password. 


## Usage
* Accessing the site
> The full url for the [website](http://ec2-35-160-130-147.us-west-2.compute.amazonaws.com) is http://ec2-35-160-130-147.us-west-2.compute.amazonaws.com
> IP address is 35.160.130.147
> SSH port is 2200

* Logging in
> Click the login button in the top right corner. You must have a [Facebook account](https://www.facebook.com) to log in.

* Logging out
> Click the logout button in the top right corner. This resets the session and clears the user.

* Editing a User
> Click the users name on the top right when logged in.
> ** Note only users can change their own information. Admins can change anyone.**
> ** Admins on this edit page will be presented with an additional 'admin console' button to view, delete and edit all users.**

**** FOR DEVELOPMENT ONLY ****
* Making a user Admin
> If you modify your nickname to "Admin" you will automatically be assigned as an admin.
******************************
* Viewing a Categories Books
> Click on the Category name

* Edit a Category
> Click on the Edit button below the Category name
> ** Note only authors of categories or admins can edit categories**

* Delete a Category
> Click on the Delete button below the Category name
> ** Note only authors of categories or admins can delete categories**

* Add a Category
> Click on the "+" button on the Category page

* View a Books information
> Click on the book image

* Edit a Book
> Click on the Edit button below the Books name
> ** Note only authors of books or admins can edit books**

* Delete a Book
> Click on the Delete button below the Books name
> ** Note only authors of books or admins can delete books**

* Checkout a Book
> If book is availible to check out there will be a check button below the book image. Click it!

* Checkin a Book
> If the book is checkout an "X" will be below the book image. Click to check in.
> ** Note only the user who checked out the book or admin can check the book back in**

## Summary of applications installed to run this project
> Apache2
> Python Setup Tools
> WSGI
> Pip
> Git
> Virtualenv
> Flask
> flask-seasurf
> httplib2
> oauth2client
> sqlalchemy
> psycopg2
> bleach
> PostgreSQL
> fail2ban

## Summary of configuation changes made to run this project
> Disabled logging in to the root user
> Disabled logging in with a password 
> Enabled a Firewall, changed SSH port to 2200 allowed HTTP and NTP
> Additional security for repeated unsuccessful logging attempts initialized with fail2ban 
> Configured the time zone to UTC
> Suppressed the Apache "Could not reliably determine the servers......" message when logging in localhost

## Summary of resources used to create this project
> [Udacity Configuring Linux Web Servers Course](udacity.com)
> [Udacity Blog to install LAMP](http://blog.udacity.com/2015/03/step-by-step-guide-install-lamp-linux-apache-mysql-python-ubuntu.html)
> [How To Secure PostgreSQL on an Ubuntu VPS](https://www.digitalocean.com/community/tutorials/how-to-secure-postgresql-on-an-ubuntu-vps)
> [How To Deploy a Flask Application on an Ubuntu VPS](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps)
> [Fail2Ban](https://www.digitalocean.com/community/tutorials/how-to-protect-ssh-with-fail2ban-on-ubuntu-14-04)
> [SQL Alchemy Docs](https://docs.sqlalchemy.org/en/latest/)
> [Stack Overflow](www.stackoverflow.com)


## Contributing

1. Email me for a user
2. Email me for a key

## Credits
Built with Flask, SQL Alchemy, Materialize JSS, Jinja,
Image from pixabay.com

## History

v1. Our first version

