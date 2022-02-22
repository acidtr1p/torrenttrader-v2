# torrenttrader-2.08

1) Copy ALL files to your webserver

2) Import via phpmyadmin "Full Database.sql"

3) Edit the file backend/mysql.php to suit your MYSQL connection

4) Edit the file backend/config.php to suit your needs
- special note should be taken for urls, emails, paths (use check.php if unsure)

5) Remove the following line from config.php: die("You didn't edit your config correctly."); // You MUST remove this line  

5) Apply the following CHMOD's
777 - cache/
777 - cache/get_row_count/
777 - cache/queries/
777 - backups/
777 - uploads/
777 - uploads/images/
777 - import/
600 - censor.txt

Edit backup-database.php and change the path. Make sure it exists and is chmod 777

if you have any of those folders missing (eg: uploads/images/), please create them and chmod 777

6) Run check.php from your browser to check you have configured everything ok
   check.php is designed for UNIX systems, if you are using WINDOWS it may not report the paths correctly.

7) Now register as a new user on the site.  The first user registered will become administrator

8) If check.php still exists, please remove it or rename.
A warning will display on the site index until its removed
