

- IOKit
- IOKit Functions
-  IOServiceAddNotification(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# IOServiceAddNotification(\_:\_:\_:\_:\_:\_:)

macOS 10.0–10.6Deprecated

``` source
func IOServiceAddNotification(
    _ mainPort: mach_port_t,
    _ notificationType: UnsafePointer!,
    _ matching: CFDictionary!,
    _ wakePort: mach_port_t,
    _ reference: UInt,
    _ notification: UnsafeMutablePointer!
) -> kern_return_t
```

