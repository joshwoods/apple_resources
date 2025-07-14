

- Application Services
- ColorSync Manager
- Color Packing for Color Spaces
-  cmOneBitDirectPacking 

Global Variable

# cmOneBitDirectPacking

One bit is used as the pixel format. This storage format is used by the resulting bitmap pointed to by the `resultBitMap` field of the function CWMatchColors; the bitmap must be only 1 bit deep.

macOS 10.0+

``` source
var cmOneBitDirectPacking: Int { get }
```

