

- Application Services
- ColorSync Manager
- Abstract Color Space Constants
-  cmHSVSpace 

Global Variable

# cmHSVSpace

An HSV color space composed of hue, saturation, and value components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

macOS 10.0+

``` source
var cmHSVSpace: Int { get }
```

