debra-create(1) -- create a new Debra directory
===============================================

## SYNOPSIS

`debra create` _name_ [_control_] [`-h`]  

## DESCRIPTION

`debra-create` creates a new Debra directory containing the skeleton of what will become a Debian package when `debra-build`(1) is run.  `DEBIAN/control` contains package metadata.  The _control_ file will be used if provided, otherwise `$HOME/.debra`, otherwise a default which will need to be filled in.

## OPTIONS

* _name_:
  Name of a Debra directory.
* [_control_]:
  Control file to use.
* `-h`, `--help`:
  Show a help message.

## FILES

* `$HOME/.debra`:
  The contents of `$HOME/.debra` will be used to initialize the `DEBIAN/control` file during the `create` action.

## THEME SONG

Beck - "Debra"

## AUTHOR

Richard Crowley <richard@devstructure.com>

## SEE ALSO

Part of `debra`(1).

`debra-create`(1), `debra-sourceinstall`(1), `debra-build`(1), `debra-destroy`(1), `debra-makefile`(1).
