<p align="center">
  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/openserver6logo.png?raw=true" />
</p>


> 1-qadam

+ OpenServer6-ni quyidagi [link](https://ospanel.io/download/) orqali yuklab olamiz va o'rnatamiz

  > Далле-ni bosamiz 

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/1.png?raw=true" />

  > Обычная установка-ni bosamiz

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/2.png?raw=true" />

  > Далле-ni bosamiz 

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/3.png?raw=true" />

  > Компактная установка-ni bosamiz. Agar sizga yana qo'shimcha narsalar kerak bo'lsa belgilab qo'shib qo'yamiz

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/4.png?raw=true" />

  > Далле-ni bosamiz

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/5.png?raw=true" />

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/6.png?raw=true" />

  > Установить-ni bosamiz

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/7.png?raw=true" />

  > Да-ni bosamiz(Sertifikatni o'rnatish)

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/8.png?raw=true" />

  > Завершить

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/9.png?raw=true" />

  > System Preparation Tool o'rnatish chiqadi. Далле-ni bosamiz

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/10.png?raw=true" />

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/11.png?raw=true" />

  > Завершить 

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/12.png?raw=true" />

  > Open Serverni ishga tushiramiz, kompyuterimiznig o'ng pastki oynasiga qaraymiz, va PhPMyAdmin yo'qligini ko'ramiz

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/14.png?raw=true" />

  > Endi phpMyAdmin-ni o'rntamiz.


<p align="center">
  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/PhpMyAdmin_log.png?raw=true", width=500/>
</p>

___

> 2-qadam

+ OpenServer6 o'rnatilgan kataolg kiramiz va undan keyin home degan katalogga kiramiz

<img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/15.png?raw=true" />

---------
---------

  > Shu katalogda phpMyAdmin degan yangi papka yaratamiz

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/16.png?raw=true" />

---------
---------

  > phpMyAdmin katalogida yana 2-ta papka yaratib olamiz. .osp va public 

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/16_.png?raw=true" />

  > .osp papkada project.ini nomli fayl yaratamiz va php-ning versiyasini va public papkani ko'rstamiz
  
  [phpMyAdmin]
  
  php_engine = PHP-7.4
  
  public_dir = {base_dir}/public

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/17.png?raw=true" />

---------
---------

  > Endi esa phpMyAdmin-ni quyidagi [link](https://www.phpmyadmin.net/) orqali yuklab olamiz va arxivdan chiqarib olamiz. Hamma fayllarni public papkaga o'tkazamiz

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/18.png?raw=true" />

---------
---------

  > config.sample.inc.php  nomli ---- faylni ---- config.inc.php  nomga o'zgartiramiz

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/19.png?raw=true" />

---------
---------

  > config.inc.php falni ochamiz va unda

---------
---------

  $cfg['blowfish_secret'] = '';  32 ta simvoldan iborat kod kiritamiz, shiftlash uchun

  $cfg['Servers'][$i]['auth_type'] = 'cookie'; ---> ni ---> $cfg['Servers'][$i]['auth_type'] = 'config';  ga o'zgartiramiz

  $cfg['Servers'][$i]['host'] = 'localhost'; ---> ni ---> $cfg['Servers'][$i]['host'] = 'MySQL-5.7'; ga o'zgartiramiz

  $cfg['Servers'][$i]['AllowNoPassword'] = false; ---> ni ---> $cfg['Servers'][$i]['AllowNoPassword'] = true; ga o'zgartiramiz

---------
---------

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/20.png?raw=true" />

---------
---------

  > Endi OpenServar6-ni qayta ishga tushiramiz

---------
---------

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/21.png?raw=true" />

  > Hamma kerakli modullarni ishga trushiramiz PHP va MySQL-ni va открыть в браузере-ni bosamiz

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/22.png?raw=true" />

  >phpMyAdmin tayyor

  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/23.png?raw=true" />

----

> Endi bemalol ma'lumotlar bazasi bilan ishlashimiz mumkin

<p align="center">
  <img src="https://github.com/DilmurodGoyupov/OpenServer_6-PhPMyAdmin-MySQL/blob/main/images/mysqllogo.png?raw=true", width=300/>
</p>
