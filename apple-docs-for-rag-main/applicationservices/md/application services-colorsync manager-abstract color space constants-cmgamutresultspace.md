

- Application Services
- ColorSync Manager
- Abstract Color Space Constants
-  cmGamutResultSpace 

Global Variable

# cmGamutResultSpace

macOS 10.0+

``` source
var cmGamutResultSpace: Int { get }
```

## Discussion

A color space for the resulting bitmap pointed to by the `resultBitMap` field of the function CWMatchColors. A bitmap never uses this constant alone. Instead, it uses the constant `cmGamutResult1Space`, which combines `cmGamutResultSpace` and `cmOneBitDirectPacking` to define a bitmap that is 1 bit deep.

