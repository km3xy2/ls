05.08 14:25
include导入文件

✔


/storage/emulated/0/nginx/b.php



/storage/emulated/0/nginx/c.php



✔


/*  ✘

/data/data/com.termux/files/
home/storage/shared/nginx/b.php



/data/data/com.termux/files/
home/storage/shared/nginx/c.php



✘   */





同级目录导入直接文件名称

include 'c.php';



或者

include  '/storage/emulated/0/nginx/c

.php';



//<?php


echo '这是c.php';


//?>


//<?php

include '/data/data/com.termux/files/home/vendor/a.php';


echo '这是b.php';

include 'c.php';


//?>


//<?php

echo "这是a.php";

//?>


'/data/data/com.termux/files/home/vendor/a.php';

访问b.php

http://127.0.0.1:8080/b.php


~ $ ls
composer-setup.php  composer.phar  vendor
composer.json       downloads      www
composer.lock       storage
~ $ ls vendor/
autoload.php  league   psr       tp5
composer      monolog  symfony
gregwar       phpu     topthink

~ $ vim vendor/a.php

~ $ php-fpm

[08-May-2021 11:41:48] NOTICE: [pool www] 'user' directive is ignored when FPM is not running as root
[08-May-2021 11:41:48] NOTICE: [pool www] 'group' directive is ignored when FPM is not running as root

~ $ nginx
~ $ php-fpm

[08-May-2021 11:42:09] NOTICE: [pool www] 'user' directive is ignored when FPM is not running as root
[08-May-2021 11:42:09] NOTICE: [pool www] 'group' directive is ignored when FPM is not running as root
[08-May-2021 11:42:09] ERROR: unable to bind listening socket for address '127.0.0.1:9000': Address already in use (98)
[08-May-2021 11:42:09] ERROR: FPM initialization failed
~ $ ls vendor/

a.php         gregwar  phpu     topthink
autoload.php  league   psr      tp5
composer      monolog  symfony
~ $






