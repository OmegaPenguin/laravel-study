# laravel-study
### day01  composer 原理
> 从composer原理出发，逐步学习laravel


#### FAQ
1. composer.lock是做什么的
composer install 命令从当前目录读取 `composer.json` 文件，处理依赖关系，并把依赖安装到vendor目录下。
如果当前目录有`composer.lock`文件，它会从此文件读取依赖版本，而不是根据`composer.json`去获取依赖。
用来确保该库的每个使用者获得相同版本的依赖
如果没有`composer.lock`，composer将在处理完依赖关系后创建它。
使用`composer update`来更新`composer.lock`中的依赖版本

2. 