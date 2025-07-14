

- IOKit
- IOKit Functions
-  IOCatalogueGetData(\_:\_:\_:\_:) 

Function

# IOCatalogueGetData(\_:\_:\_:\_:)

macOS 10.0+

``` source
func IOCatalogueGetData(
    _ mainPort: mach_port_t,
    _ flag: UInt32,
    _ buffer: UnsafeMutablePointer?>!,
    _ size: UnsafeMutablePointer!
) -> kern_return_t
```

