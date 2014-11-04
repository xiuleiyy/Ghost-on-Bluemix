Ghost
===================
Ghost is a free, open, simple blogging platform that's available to anyone who wants to use it. Lovingly created and maintained by John O'Nolan + Hannah Wolfe + an amazing group of contributors.

Visit the project's website at http://ghost.org • docs on http://support.ghost.org.

Ghost-on-Bluemix
================

Run Ghost on Bluemix with local-file-store type

The code has been modified to run on Bluemix with local-file-store type. In the future, will add DB support and all the files and pics will store in DB, when you restart the app, all the files and pics will be kept.

How to run Ghost on Bluemix?
==================================
1. Download all the files and extract to your local machine, eg C:/ghost
2. Open config.js, thre is one line in 'production' section like below:
url: 'http://ghostonbxen.mybluemix.net',
Change the url value to your actual host and domain when you deploy it to Bluemix. For example, if you want to deploy this app with name "ghostblog", you need to change the url to 'http://ghostblog.mybluemix.net'
3. Install Cloud Foundry CLI and connect to IBM Bluemix, from the app root directory run "cf push ghostblog" to push app to Bluemix
4. Access http://ghostblog.mybluemix.net/ghost/setup to register with administrator and start to write your blog.
5. You can view your blogs by http://ghostblog.mybluemix.net
6. The other url you can relogin http://ghostblog.mybluemix.net/ghost/signin/ if you already log out.
