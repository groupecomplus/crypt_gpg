# Crypt_GPG #
Crypt_GPG is a PHP package to interact with the [GNU Privacy Guard 
(GnuPG)](http://www.gnupg.org/). GnuPG is a free and open-source
implementation of the [OpenPGP](http://www.ietf.org/rfc/rfc4880.txt)
protocol, providing key management, data encryption and data signing.
Crypt_GPG provides an object-oriented API for performing OpenPGP
actions using GnuPG.

[Crypt_GPG](http://pear.php.net/package/Crypt_GPG) has been
migrated from [PEAR SVN](https://svn.php.net/repository/pear/packages/Crypt_GPG).

## Documentation ##

### Quick Example
```php
<?php

require_once 'Crypt/GPG.php';

$gpg = new Crypt_GPG();
$gpg->addEncryptKey('test@example.com');
$data = $gpg->encrypt('my secret data');

?>
```

### Further Documentation ###
* [High-Level Documentation](http://pear.php.net/manual/en/package.encryption.crypt-gpg.intro.php)
* [Detailed API Documentation](http://pear.php.net/package/Crypt_GPG/docs/latest/)

## Bugs and Issues ##
Please report all new issues via the [PEAR bug tracker](http://pear.php.net/bugs/search.php?cmd=display&package_name[]=Crypt_GPG).

Please submit pull requests for your bug reports!

## Testing ##
To test, run either
$ phpunit tests/
  or
$ pear run-tests -r

## Building ##
To build, simply
$ pear package

## Installing ##
To install from scratch
$ pear install package.xml

To upgrade
$ pear upgrade -f package.xml
