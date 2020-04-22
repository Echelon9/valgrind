# Valgrind for macOS

This repository contains a version of Valgrind including a few patches to improve support for the macOS platform.

## Status

Valgrind now builds on macOS Mojave (tested on 10.14.6) & Catalina (tested 10.15.1 & 10.15.4).

## Usage

In order to use this version, use the following command:

```
brew install --HEAD https://raw.githubusercontent.com/sowson/valgrind/master/valgrind.rb
```

In case you already have Valgrind installed, you will need to either `unlink` it first or `reinstall` it.

## CLion

Valgridn executable:
/usr/local/bin/valgrind

Analysis options:
--leak-check=full --leak-resolution=med --track-origins=yes --vgdb=no

For testing/developing/checking:
--trace-syscalls=yes

