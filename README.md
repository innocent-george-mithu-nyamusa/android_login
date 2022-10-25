## Steps for setting up
  - Git clone this Repository
  - Copy android_login folder to XAMPP=>htdocs
  - Create database android_login =>

         create table users( id int(11) primary key auto_increment, unique_id varchar(23) not null unique, name varchar(50) not null, email varchar(100) not null unique, encrypted_password varchar(250) not null, otpint(6) NOT NULL, verified int(1) NOT NULL DEFAULT '0', created_at datetime DEFAULT NULL );

  - Change Config.php file for username and password
      
      $username = "root"; 
      $password = ""; 
      $host = "localhost"; 
      $dbname = "android_login"; 

  - Change Main Url inside Functions.Java File 
  - If you are using localhost:[PORT] change Mainurl to MAIN_URL = "http://localhost:[PORT]/android_login/"
  - If you are using just localhost change Mainurl to MAIN_URL = "http://localhost/android_login/"

