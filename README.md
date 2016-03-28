# ZKLibrary
ZKLibrary is PHP library for reading and writing data to attendance device using UDP protocol. This library is useful to comunicate between web server and attendance device directly without any addition program.
This library is implemented in the form of class. So that you can create an object and use it functions.

## Example

<?php

include "zklibrary.php";

$zk = new ZKLibrary('192.168.1.102', 4370);

$zk->connect();

$zk->disableDevice();

$zk->testVoice();

$zk->enableDevice();

$zk->disconnect();

?>
