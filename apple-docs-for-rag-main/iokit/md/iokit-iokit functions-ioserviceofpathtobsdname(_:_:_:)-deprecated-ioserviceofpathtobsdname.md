

- IOKit
- IOKit Functions
-  IOServiceOFPathToBSDName(\_:\_:\_:) Deprecated

Function

# IOServiceOFPathToBSDName(\_:\_:\_:)

macOS 10.0–10.8Deprecated

``` source
func IOServiceOFPathToBSDName(
    _ mainPort: mach_port_t,
    _ openFirmwarePath: UnsafePointer!,
    _ bsdName: UnsafeMutablePointer!
) -> kern_return_t
```

