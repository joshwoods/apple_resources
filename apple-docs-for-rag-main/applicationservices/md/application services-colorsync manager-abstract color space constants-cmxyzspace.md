

- Application Services
- ColorSync Manager
- Abstract Color Space Constants
-  cmXYZSpace 

Global Variable

# cmXYZSpace

An XYZ color space composed of X, Y, and Z components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

macOS 10.0+

``` source
var cmXYZSpace: Int { get }
```

