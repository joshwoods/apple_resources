

- Foundation
- Data
- Data.Deallocator
-  Data.Deallocator.custom(\_:) 

Case

# Data.Deallocator.custom(\_:)

A custom deallocator.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case custom((UnsafeMutableRawPointer, Int) -> Void)
```

## See Also

### Enumeration Cases

case free

Use `free`.

case none

Do nothing upon deallocation.

case unmap

Use `munmap`.

case virtualMemory

