

- Application Services
- ColorSync Manager
- Abstract Color Space Constants
-  cmHLSSpace 

Global Variable

# cmHLSSpace

An HLS color space composed of hue, lightness, and saturation components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

macOS 10.0+

``` source
var cmHLSSpace: Int { get }
```

