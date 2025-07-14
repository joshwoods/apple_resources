

- Application Services
- ColorSync Manager
- Abstract Color Space Constants
-  cmRGBASpace 

Global Variable

# cmRGBASpace

macOS 10.0+

``` source
var cmRGBASpace: Int { get }
```

## Discussion

An RGB color space composed of red, green, and blue color value components and an alpha channel component. ColorSync does not currently support bitmaps that use this constant alone. Instead, this constant indicates the presence of an alpha channel in combination with `cmLong8ColorPacking` to indicate 8-bit packing format and `cmAlphaFirstPacking` to indicate the position of the alpha channel as the first component.

