# RDFBrowser
A Linked Data content negotiation and publication platform coded in PHP for consumer level applications.

#Installation instructions
This is an application developed with Laravel MVC PHP Framework. Follow these instructions to succesfully install the app.

```sh
#clone the repo on a folder of your choice, usually /home/$user

$ git clone https://github.com/okgreece/RDFBrowser.git

$ cd RDFBrowser

# build dependencies
$ composer install

# copy default settings SQLite database on storage folder
$ cp setup/database.sqlite storage/database.sqlite

#copy or move folder on your public folder usually /var/www 
$ cd ..
$ cp RDFBrowser/ /var/www/RDFBrowser

#...or create a simlink to it

#finally, copy .htaccess settings file to root of your public folder, usually /var/www
$ cp /var/www/RDFBrowser/setup/.htaccess /var/www/.htaccess

```

Please, take care to make appropriate changes when you use different folders, or if you don't have wright permissions on the public folder. 

Go to http://yourdomain/admin. It will redirect you at the login page. 

Use username : admin@admin.com
        pass : admin1
        
Remember to change these settings after first login.

Then go to Endpoint section. It defaults to DBpedia SPARQL Endpoint as NON working example. You should change at least the URL of your Endpoint to reflect your configuration. 

Enjoy your new Linked Data Application!!!

#Quickstart & Shared Hosting

You can choose the pre-built releases on [Pre-Built Realeses and Source Code](https://github.com/okgreece/RDFBrowser/releases/) if you want to quickstart your new app. Just extract the zipped files, change Endpoint AND User Login settings and you are ready to go!
