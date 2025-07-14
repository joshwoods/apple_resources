

- IOKit
- IOKit Functions
-  IORegistryEntryCopyFromPath(\_:\_:) 

Function

# IORegistryEntryCopyFromPath(\_:\_:)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func IORegistryEntryCopyFromPath(
    _ mainPort: mach_port_t,
    _ path: CFString!
) -> io_registry_entry_t
```

