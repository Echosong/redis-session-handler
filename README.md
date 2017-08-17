# redis-session-handler

Quick Start

Download and install

  install php  extension for redis  http://pecl.php.net/package/redis
  
Composer package

  composer require echosong/redisSession
 
Use
    ```php
    
    $config =[
           'host'=>'127.0.0.1',
           'port'=> 6379,
           'timeout'=>2,
          'auth'=>'****',
          'database'=>2,
          'prefix' => 'redis_session:'
      ]
    session_set_save_handler(new \Echosong\RedisSession\RedisSessionHandler($config), true);
    session_start();
    ```

