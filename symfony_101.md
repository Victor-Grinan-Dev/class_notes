# symfony 101

## install symfony:
-   for mac:
    ```shell
    brew install symfony-cli/tap/symfony-cli
    ```
-   for pc:
    ```shell
    scoop install symfony-cli
    ```
    
    or:
    
    ```shell
    gofish rig add https://github.com/symfony-cli/fish-food
    gofish install github.com/symfony-cli/fish-food/symfony-cli
    ```
    
 ## create a new symfony app:
 
 -  for big project:
     ```shell
     symfony new my_project --webapp 
     ```
     
  -  for small project:
     ```shell
     symfony new my_project (not recomended for this steps)
     ```
     
 ## run webserver:  
 
 ```shell
 symfony server:start 
 ```
     
 ## if your are using database:
 
  ```shell
 composer require symfony/maker-bundle --dev
 
 composer require orm 
 ```
 type yes to everything.
 
 now to make the entitie ("tables") of database:
   ```shell
 composer require symfony/maker-bundle --dev
 
 composer require orm 
 ```
 bin/console make:entity  

     
  

  
  ```shell
  symfony serve -d
  ```
  copy the url in the green square an paste it in the browser
  ```shell
  https://127.0.0.1:8000 
  ```
To install dependencies run:
```shell
composer requiere name-of-library 
```

To check if updates are avilable to your recipes:
```shell
composer recipes
```

If the recipes have a little update available in the side means they need update.
To update this recipes run:
```shell
composer recipes:update
```

database:
-   make sure you have orm
    ```shell
    composer require orm
    ```
-   make sure you have docker installed

entity:
-   make sure you have orm
    ```shell
    bin/console make entity
    ```
