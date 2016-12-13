# Additional Particle build tools for Windows

The crc32.exe and xxd.exe tools needed for Particle gcc-arm local build on Windows.

Pre-built binaries for Cygwin 32-bit and 64-bit and MinGW 32-bit are included. (I had trouble installing the MinGW 64-bit gcc compiler so that one is missing. Maybe you'll have better luck.)

If you want to build them manually from source, use commands like:

```
gcc -o crc32.exe crc32.c
gcc -o xxd.exe xxd.c -DCYGWIN
```

Specify `-DCYGWIN` even for MinGW.


### crc32

[https://opensource.apple.com/source/xnu/xnu-1456.1.26/bsd/libkern/crc32.c](https://opensource.apple.com/source/xnu/xnu-1456.1.26/bsd/libkern/crc32.c)

> COPYRIGHT (C) 1986 Gary S. Brown.  You may use this program, or
> code or tables extracted from it, as desired without restriction.

### xxd

[https://opensource.apple.com/source/vim/vim-44/src/xxd/xxd.c](https://opensource.apple.com/source/vim/vim-44/src/xxd/xxd.c)

> (c) 1990-1998 by Juergen Weigert (jnweiger@informatik.uni-erlangen.de)
>  Small changes made afterwards by Bram Moolenaar et al.
> 
>  Distribute freely and credit me,
>  make money and share with me,
>  lose money and don't ask me.
  