> 此项目是php-angular在thinkphp5中使用的驱动, 可在tp5项目中使用composer安装, 安装后配置模板引擎为`Angular`即可.  

## 1. 安装composer

教程: http://www.phpcomposer.com

## 2. 安装驱动  
```
composer require php-angular/thinkphp:2.0.*
```

## 3. 修改或添加项目配置文件的模板引擎为Angular  

// 修改配置文件 /config/template.php
```
use think\facade\Env;

return [
    // 模板引擎类型 支持 php think Angular 支持扩展
    'type'             => 'Angular',
    'debug'            => true, // 是否开启调试模式
    'tpl_suffix'       => '.html', // 模板后缀
    'tpl_cache_suffix' => '.php', // 模板缓存文件后缀
    'directive_prefix' => 'php-', // 指令前缀
    'directive_max'    => 10000, // 指令的最大解析次数
];

```

## 资源教程

1. 核心模板解析库: https://github.com/php-angular/php-angular  
2. thinkphp5: https://github.com/top-think/think
