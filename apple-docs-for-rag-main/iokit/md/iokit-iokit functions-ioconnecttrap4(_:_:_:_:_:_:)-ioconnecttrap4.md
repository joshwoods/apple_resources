

- IOKit
- IOKit Functions
-  IOConnectTrap4(\_:\_:\_:\_:\_:\_:) 

Function

# IOConnectTrap4(\_:\_:\_:\_:\_:\_:)

macOS 10.0+

``` source
func IOConnectTrap4(
    _ connect: io_connect_t,
    _ index: UInt32,
    _ p1: UInt,
    _ p2: UInt,
    _ p3: UInt,
    _ p4: UInt
) -> kern_return_t
```

