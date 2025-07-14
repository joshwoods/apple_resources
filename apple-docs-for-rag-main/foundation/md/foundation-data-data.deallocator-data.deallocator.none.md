

- Foundation
- Data
- Data.Deallocator
-  Data.Deallocator.none 

Case

# Data.Deallocator.none

Do nothing upon deallocation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case none
```

## See Also

### Enumeration Cases

case custom((UnsafeMutableRawPointer, Int) -> Void)

A custom deallocator.

case free

Use `free`.

case unmap

Use `munmap`.

case virtualMemory

