

- Application Services
- ColorSync Manager
- Abstract Color Space Constants
-  cmYXYSpace 

Global Variable

# cmYXYSpace

A Yxy color space composed of Y, x, and y components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

macOS 10.0+

``` source
var cmYXYSpace: Int { get }
```

