# Exit Codes

This article will inform you about the error codes.

**Warning:** Unless you code the `*.cmm` file to exit with that specific code, the compiler should normally not exit with these numbers. If it does, that means there is an error on the compilers code or the `*.cmm` file.

## 0x00 or 0

Unless you specifically coded to exit with this number, this exit code means the file does not exist. C-- will create a blank output file that just returns zero and then run it.

## 0x7F or 127

Unless you modified the compiler code, this means a bug in the code. Please create an issue at https://github.com/XarCraftCoding/C--/issues/new.

## Any Unwanted Exit Code

**_Before Reading:_** `integer limit (8-bit)` is 256.

These exit codes mean the compiler tried to return negative numbers. Because it can't return negative numbers, it returned `integer limit (8-bit) + remaining from subtraction`, in this case remaining is negative; so we subtract our negative number from `256` and that will give us the exit code.
