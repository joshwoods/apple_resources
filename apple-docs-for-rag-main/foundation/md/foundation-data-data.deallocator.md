

- Foundation
- Data
-  Data.Deallocator 

Enumeration

# Data.Deallocator

A deallocator you use to customize how the backing store is deallocated for data created with the no-copy initializer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Deallocator
```

## Topics

### Enumeration Cases

case custom((UnsafeMutableRawPointer, Int) -> Void)

A custom deallocator.

case free

Use `free`.

case none

Do nothing upon deallocation.

case unmap

Use `munmap`.

case virtualMemory

## See Also

### Creating Data from Raw Memory

init(bytes: UnsafeRawPointer, count: Int)

Creates data with copied memory content.

init&lt;SourceType>(buffer: UnsafeBufferPointer&lt;SourceType>)

Creates a data buffer with copied memory content using a buffer pointer.

init&lt;SourceType>(buffer: UnsafeMutableBufferPointer&lt;SourceType>)

Creates a data buffer with copied memory content using a mutable buffer pointer.

init(bytesNoCopy: UnsafeMutableRawPointer, count: Int, deallocator: Data.Deallocator)

Creates a data buffer with memory content without copying the bytes.

