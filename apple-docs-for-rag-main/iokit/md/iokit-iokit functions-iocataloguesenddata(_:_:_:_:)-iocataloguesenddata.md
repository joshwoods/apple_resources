

- IOKit
- IOKit Functions
-  IOCatalogueSendData(\_:\_:\_:\_:) 

Function

# IOCatalogueSendData(\_:\_:\_:\_:)

macOS 10.0+

``` source
func IOCatalogueSendData(
    _ mainPort: mach_port_t,
    _ flag: UInt32,
    _ buffer: UnsafePointer!,
    _ size: UInt32
) -> kern_return_t
```

