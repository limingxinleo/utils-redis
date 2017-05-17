# Redis单例类

## Composer 安装
~~~
composer require limingxinleo/utils-redis
~~~

## 使用方法
~~~
$redis = \limx\utils\Redis::getInstance(
    $config->redis->host,
    $config->redis->auth,
    $config->redis->index,
    $config->redis->port
);

print_r($redis->keys("*"));
~~~