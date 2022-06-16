# Java class file version

## Magic number

First four bytes of every `.class` is `CA FE BA BE`, then 2 bytes minor version (until now, always zero), then 2 bytes major version.

## Class file format version

From [Wikipedia](https://en.wikipedia.org/wiki/Java_class_file#Magic_Number):

```
Java SE 18  = 62 (0x3E hex),
Java SE 17  = 61 (0x3D hex),
Java SE 16  = 60 (0x3C hex),
Java SE 15  = 59 (0x3B hex),
Java SE 14  = 58 (0x3A hex),
Java SE 13  = 57 (0x39 hex),
Java SE 12  = 56 (0x38 hex),
Java SE 11  = 55 (0x37 hex),
Java SE 10  = 54 (0x36 hex),
Java SE 9   = 53 (0x35 hex),
Java SE 8   = 52 (0x34 hex),
Java SE 7   = 51 (0x33 hex),
Java SE 6.0 = 50 (0x32 hex),
Java SE 5.0 = 49 (0x31 hex),
JDK 1.4     = 48 (0x30 hex),
JDK 1.3     = 47 (0x2F hex),
JDK 1.2     = 46 (0x2E hex),
JDK 1.1     = 45 (0x2D hex).
```

> See the original Wikipedia article, it contains more useful/interesting information.

### Example

```
00000000: CA FE BA BE 00 00 00 34|03 49 0A 01 08 01 C2 09
```

that means this .class was compiled with Java SE 8.
