

- Application Services
- ColorSync Manager
- Abstract Color Space Constants
-  cmRGBSpace 

Global Variable

# cmRGBSpace

An RGB color space composed of red, green, and blue components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

macOS 10.0+

``` source
var cmRGBSpace: Int { get }
```

