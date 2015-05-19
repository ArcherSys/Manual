# For Developers

## How do you develop for ArcherSys OS?

The Philosophy is simple : Use the View.

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
