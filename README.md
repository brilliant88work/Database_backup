# Database_backup
1. You can install the package via composer:

composer require spatie/db-dumper

2. Download the BackupController.php
 - Save in the app>Http>Controllers 
 - Change that 4 values accoding to your project
  1. $mysql_path = string
  2. $user_name = string
  3. $pass_word = string
  4. $data_base = array

3. Write the below route in web.php
 - Route::get('/', 'BackupController@index');
 - Route::get('/databackup', 'BackupController@dataBackup')->name('databackup');
 - Route::post('/databackup', 'BackupController@dataBackup')->name('databackup');

4. Download the dbbackup folder
 -  Save the folder in resources>views
