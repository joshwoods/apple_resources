

- Application Services
- ColorSync Manager
- Abstract Color Space Constants
-  cmLABSpace 

Global Variable

# cmLABSpace

An L\*a\*b\* color space composed of L\*, a\*, b\* components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

macOS 10.0+

``` source
var cmLABSpace: Int { get }
```

