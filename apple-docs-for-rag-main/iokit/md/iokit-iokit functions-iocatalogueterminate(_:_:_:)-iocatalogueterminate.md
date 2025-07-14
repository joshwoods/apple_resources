

- IOKit
- IOKit Functions
-  IOCatalogueTerminate(\_:\_:\_:) 

Function

# IOCatalogueTerminate(\_:\_:\_:)

macOS 10.0+

``` source
func IOCatalogueTerminate(
    _ mainPort: mach_port_t,
    _ flag: UInt32,
    _ description: UnsafeMutablePointer!
) -> kern_return_t
```

