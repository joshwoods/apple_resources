

- IOKit
- IOKit Functions
-  IORegistryEntryGetProperty(\_:\_:\_:\_:) 

Function

# IORegistryEntryGetProperty(\_:\_:\_:\_:)

macOS 10.0+

``` source
func IORegistryEntryGetProperty(
    _ entry: io_registry_entry_t,
    _ propertyName: UnsafePointer!,
    _ buffer: UnsafeMutablePointer!,
    _ size: UnsafeMutablePointer!
) -> kern_return_t
```

