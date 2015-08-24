# wordpressinstallationsystem
Automatically exported from code.google.com/p/wordpressinstallationsystem



---


---

> # Wordpress Installation System #

https://github.com/speedily/wordpressinstallationsystem
---


---

## by Abhishek Jha ##
http://abhishekjha.net/

---


### Intro: ###
Wordpress Installation System(WPIS) is a php/mysql based Wordpress Installation Automation and Controlled Installation System for Web Hosting providers. If you are a web hosting provider and would like to automate your task of providing people a ready made website of their needs, then this script makes it easy for you to make a user system controllable from admin panel or db which can be modified by your billing software to create a user a/c with a domain name, number of installations he can do on that domain, the kind of website he can make like blog, support forum, site, news portal etc using the power of WordPress and its plugins. It will allow user to choose between ready made templates and the user will just enter their details and have their website of their choice installed on their domain and controllable via their WordPress admin panel.

### Usage Case-Study: ###
Assume that you are a web hosting provider who wants to offer something new to his clients, that is a service to enable the clients to make ready-made websites at the press of a button. So you have WHMCS(or some billing software) on the front end and Cpanel on backend on a LAMP stack. Now users who come to your site buy a domain, then buy hosting and also add a ready made blog site with some template design and features, the domain and hosting you can manage with whmcs, but the site development is the manual task almost everywhere, but if you use WPIS along with WHMCS integration then you can have a package of a blog with some plugins and a choice of templates to the client. The clients a/c you can make via WPIS admin panel or automatedly via WHMCS + php script to work on WPIS and create a WPIS user a/c. Now the user is provided with a Login ID and Authentication code and his a/c is limited to a domain(set by you) and the number of times(via balance points system) he can install the blog on that domain via WPIS front-end and the names and selection of plugins he can choose from on the installation system. Once the user's a/c is created via WPIS admin, he is sent an e-mail and told to goto WPIS frontend where he can enter the Login/Auth. Code and Install his blog on his domain by just entering a few details(like mysql, template choice, plugin choice, etc) and pressing "Install" button.


---

Note: Tested only on linux server on php 5.2 with - zip option(req. specially on target server where user is gonna install wordpress using WPIS) and mysql db.

---

### Install Steps: ###
<br />1.Extract the zip "wpisredist.zip" to any folder under your domain's root (the folder from where you want it to run)
<br />2.Find the "wpinstallationdump20feb2011.sql" file under "readme" folder and import it into your mysql database
<br />3.Open "config.php" and set the dbname, password etc settings
<br />4.Lastly .. You may have to modify the php sent e-mail message in "installsuccess.php" and in admin folder's "add.php",  to match the description of your domain, from and ending line so that your users come to the correct server to WPIS front-end  and also you can change the logo by changing the "images/wpis.png" image.
<br />..thats it!

### Usage: ###
<br />1.Goto yourinstalleddomain/admin  and use ID/PASS as admin/admin
<br />2.Setup user a/c or use existing user a/c on your script home page yourinstalleddomain, user is sent and e-mail after a/c is added and thus you get.
<br />3.Now you enter the user's server etc details in the form and can install wordpress with plugins/templates on the user's domain at the press of a button

If you have any other problems, ideas for improvement, or you may wanna donate, then either:
<br /> Reach on our project page https://github.com/speedily/wordpressinstallationsystem
or
<br /> Contact me on http://abhishekjha.net/ or use github issues.

### Copyright ###
Its GNU GPL2(same as that of Wordpress Itself). See "license.txt" inside the zip file for more info.
