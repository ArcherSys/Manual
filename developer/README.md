# For Developers

## How do you develop for ArcherSys OS?

The Philosophy is simple : Use the View.

!FILENAME example.php

```
<?php
require_once $_SERVER["DOCUMENT_ROOT"]."\includes\View.php";
use ArcherSys\Viewer\Contrib\View;
$view = new View("Example", function(){
?>
<meta name="author" content="John Doe">
<?php

},function(){
?>
<h1>Hello World</h1>
<?php
});
?>
```
Another Example uses Bootstrap:
```
<?php
  require_once $_SERVER["DOCUMENT_ROOT"]."\includes\View.php";
  use ArcherSys\Viewer\Contrib\View;
  $bootstrap_view = new View("My Bootstrap View",function(){
  ?>
 //Use bootstrap Resources Here
 <?php
    , function(){
    $container = new Container(function(){
     ?>
     <!---Content Here-->
     <?php
     });
     });
     ?>
     
  
?>
```
Another Thing You Can Do in the Head Tag:
```
<?php
require_once $_SERVER["DOCUMENT_ROOT"]."\includes\View.php";
use ArcherSys\Viewer\Contrib\View;
$view = new View("Example", function(){
DescriptionManager::addAuthor("John Doe");

},function(){
?>
<h1>Hello World</h1>
<?php
});
?>
```

This is the first Container Component to go in this API.
To Develop in Python go [here](lib_cmd.md)
