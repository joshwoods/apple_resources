

- Foundation
- Data
- Data.Deallocator
-  Data.Deallocator.free 

Case

# Data.Deallocator.free

Use `free`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case free
```

## See Also

### Enumeration Cases

case custom((UnsafeMutableRawPointer, Int) -> Void)

A custom deallocator.

case none

Do nothing upon deallocation.

case unmap

Use `munmap`.

case virtualMemory

