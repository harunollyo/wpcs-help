### 1. Install the composer package
```    
composer global require squizlabs/php_codesniffer
```
```
composer global require wp-coding-standards/wpcs
```
    
**Installation Test**
    
``` 
phpcs -i
```

`phpcs` and `phpcbf` installed path.  
  
/Users/your_username/.composer/vendor/bin/phpcs  
/Users/your_username/.composer/vendor/bin/phpcbf  

[Note] change  `your_username`

### 2. Set WordPress as default coding standards
[Note] change `your_username`
    
```
phpcs --config-set installed_paths /Users/your_username/.composer/vendor/wp-coding-standards/wpcs
```

**Installation Test**  
    
```
phpcs --config-show
```

### 3. For validate your php file
    
```
phpcs abc.php
```

### 4. For automatic fix, run

```
phpcbf abc.php
```
