# How to setup Laravel Framework
  ## Windows Enviroment
  ### Download and install the following; 
 1. https://www.apachefriends.org/index.html - PHP, MYSql, etc.
  * Download and install XAMPP
  * Follow prompts to install
  * You dont need Bitnami at this time
  * Ensure PHP is installed at command line
  * Launch System Window --> System Properties --> Advanced Tab
  * Under System Varaiables, find and edit "PATH"
  * Add the path of the PHP folder to the edit of the Variable value: (i.e. ;C:\xampp\php)
  * To test if done correctly, launch CMD (command prompt) and type "php -v"
           
 2. https://getcomposer.org/ - dependency manager for PHP
  * Download and install Composer
  * Point to the PHP folder (should automatically do this)
  * To test installation, go to CMD (comand prompt) and type "composer -v"
  * To update (if needed) type "composer self-update"
  * Otherwise add additional plug-ins
    * Type "composer global require fxp/composer-asset-plugin"
       
 3. https://git-scm.com/downloads - Managing code repositories
  * Download and install git
  * Follow prompts, default setting are fine for now
  * to test if installed corrected, launch CMD (command prompt) and type "git --version"
  
  4. Finishing up
   * Navigate and open "php.ini" in the php folder
   * Uncomment international extention by searching document for "intl"
     * Delete ";" from begining of line, or uncomment "extention-php_intl.dll"
   * Set server timezone by searching document for "timezone" 
     * Delete ";" from beginning of line, or uncomment "date.timezone ="
     * Go to URL http://php.net/date.timezone
     * Click "List of supported timezones"
     * Copy and past "location" after the "date.timezone ="
     
  5a. Install Laravel from Composer
   * Create a new directory where ever you want, but if running XAMPP, the root directory would be best.
   * Using CMD, navigate and create a directory
   * Type "composer create-project --prefer-dist laravel/laravel"
   * Type "php artisan serve"
     *** POSSIBILITY - Might have to navigate to App directory first ***
  5.b Additional Flexability
    * Type "cd app" to root of Laravel App
    * Type "php artisan list"
      * This will show a list of commands available inside Artisan
      
   
 ## After setup and running
   1. 
