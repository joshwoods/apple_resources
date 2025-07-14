

- Application Services
- ColorSync Manager
- Abstract Color Space Constants
-  cmCMYKSpace 

Global Variable

# cmCMYKSpace

A CMYK color space composed of cyan, magenta, yellow, and black. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

macOS 10.0+

``` source
var cmCMYKSpace: Int { get }
```

