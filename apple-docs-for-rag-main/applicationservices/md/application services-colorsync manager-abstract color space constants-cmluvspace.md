

- Application Services
- ColorSync Manager
- Abstract Color Space Constants
-  cmLUVSpace 

Global Variable

# cmLUVSpace

An L\*u\*v\* color space composed of L\*, u\*, and v\* components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

macOS 10.0+

``` source
var cmLUVSpace: Int { get }
```

