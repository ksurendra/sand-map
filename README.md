sand-map
=============

Visualize locations as markers on a custom Google Map. Host everything locally on your own server, or optionally show data from database

Requirements
------------

- PHP5
- MySQL


Installation
------------

Setup should be super easy. Follow these steps:

1. Create a new MySQL database and user.
2. Use phpMyAdmin or another MySQL utility to run each of the SQL files in the /db directory.
3. Open /include/db_example.php with your text editor. Enter your MySQL credentials in there. Also, replace "letsgetmappy" with a new password for the admin panel. Rename the file to "db.php".
4. Upload all of the files to your server.
5. You'll probably want to comb through index.php with your favorite text editor and replace all the RepresentLA content
   (logo, "more info" text, Twitter/Facebook share buttons, etc.) with your own stuff.
6. Populate your database. We recommend seeding it with some existing data before opening it up to your local community.
   You can add markers by using the button on the map page, or by importing them with an SQL query. If you use an SQL
   query, note that you should leave the lat/long values blank when importing. Then, run geocode.php to automatically
   generate lat/long values for all your rows.
7. Once visitors to your site have submitted their own markers, point your browser to /admin to approve/reject them.
8. Challenge your newly-discovered neighbors to ping pong!
