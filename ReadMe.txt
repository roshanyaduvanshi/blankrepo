Author: CodexWorld
Author URL: http://www.codexworld.com/
Author Email: contact@codexworld.com
Tutorial Link: http://www.codexworld.com/server-side-filtering-jquery-ajax-php-mysql/

============ Instruction ============
1. Create a database (for example, codexworld) and import the "users.sql" file into this database.
2. Open the "DB.php" file => change the $dbHost, $dbUsername, $dbPassword, and $dbName variable's value as per your phpMyAdmin details.
3. Browse the "index.php" file on the browser. In this page, you'll see the users data listed from the database with search and filtering option.


============ May I Help You ===========
If you have any query about this script, send us by posting a comment here - http://www.codexworld.com/server-side-filtering-jquery-ajax-php-mysql/#respond




<?php
					$objectManagerlogin = \Magento\Framework\App\ObjectManager::getInstance();
					$customerSession = $objectManagerlogin->get('Magento\Customer\Model\Session');
					$baseurl = $objectManagerlogin->get('Magento\Store\Model\StoreManagerInterface')->getStore(0)->getBaseUrl();
				?>