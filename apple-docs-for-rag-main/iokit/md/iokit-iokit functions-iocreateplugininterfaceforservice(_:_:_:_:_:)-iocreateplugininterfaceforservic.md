

- IOKit
- IOKit Functions
-  IOCreatePlugInInterfaceForService(\_:\_:\_:\_:\_:) 

Function

# IOCreatePlugInInterfaceForService(\_:\_:\_:\_:\_:)

Mac Catalyst 13.0+macOS 10.0+

``` source
func IOCreatePlugInInterfaceForService(
    _ service: io_service_t,
    _ pluginType: CFUUID!,
    _ interfaceType: CFUUID!,
    _ theInterface: UnsafeMutablePointer?>?>!,
    _ theScore: UnsafeMutablePointer!
) -> kern_return_t
```

