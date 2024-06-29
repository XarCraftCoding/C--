# C-- Exit Codes

This article will inform you about the error codes.

**Warning:** Unless you code the `*.cmm` file to exit with that specific code, the compiler should normally not exit with these numbers. If it does, that means there is an error on the compilers code or the `*.cmm` file.

## 0x00 or 0

This exit code means no exit code is inputted or the file does not exist, thus C-- will create a blank output file that just returns zero and then run it.

## 0x7F or 127

Unless you modified the compiler code, this means a bug in the compilers original code. Please create an issue at https://github.com/XarCraftCoding/C--/issues/new.

## Any Unwanted Exit Code

**_Before Reading:_** `integer limit (8-bit)` is 256.

These exit codes mean the compiler tried to return negative numbers or numbers bigger than `integer limit (8-bit)`. Because it can't return negative numbers or numbers bigger than `integer limit  (8-bit)`, it returns `<inserted value> modded by integer limit (8-bit)`.