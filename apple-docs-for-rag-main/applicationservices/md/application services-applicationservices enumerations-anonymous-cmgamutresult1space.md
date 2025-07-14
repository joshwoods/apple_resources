

- Application Services
- ApplicationServices Enumerations
- Anonymous
-  cmGamutResult1Space 

Global Variable

# cmGamutResult1Space

macOS 10.0+

``` source
var cmGamutResult1Space: Int { get }
```

## Discussion

A gamut result color space for the resulting bitmap pointed to by the `resultBitMap` field of the function CWMatchColors, with 1-bit direct packing. A pixel in the returned bitmap with value 1 (displayed as black) indicates an out-of-gamut color, while a pixel value of 0 (white) indicates a color that is in gamut.

