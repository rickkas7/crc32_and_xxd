# crc32_and_xxd

These two tools needed for Particle gcc-arm local build on Windows.

You'll need to build them for Cygwin or MinGW, depending on what you have installed. For example:

```
gcc -o crc32.exe crc32.cpp
gcc -o xxd.exe xxd.cpp -DCYGWIN
```
