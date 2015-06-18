# Flysystem Adapter for Icewind SMB

## To-do:

* Write tests.

## Usage
```php
use Icewind\SMB\Server;
use League\Flysystem\Filesystem;
use RobGridley\Flysystem\Smb\SmbAdapter;

$server = new Server('host', 'username', 'password');
$share = $server->getShare('name');

$filesystem = new Filesystem(new SmbAdapter($share));
```
## Installation
```
$ composer require 'robgridley/flysystem-smb:dev-master'
$ composer update
```
