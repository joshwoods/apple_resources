

- Foundation
- Data
-  init(bytes:count:) 

Initializer

# init(bytes:count:)

Creates data with copied memory content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    bytes: UnsafeRawPointer,
    count: Int
)
```

## Parameters 

`bytes`  

A pointer to the memory to copy.

`count`  

The number of bytes to copy.

## See Also

### Creating Populated Data

init()

Creates an empty data buffer.

init&lt;S>(S)

Creates a new instance of a collection containing the elements of a sequence.

init&lt;SourceType>(buffer: UnsafeBufferPointer&lt;SourceType>)

Creates a data buffer with copied memory content using a buffer pointer.

init&lt;SourceType>(buffer: UnsafeMutableBufferPointer&lt;SourceType>)

Creates a data buffer with copied memory content using a mutable buffer pointer.

init(bytesNoCopy: UnsafeMutableRawPointer, count: Int, deallocator: Data.Deallocator)

Creates a data buffer with memory content without copying the bytes.

init(capacity: Int)

Creates an empty data buffer of a specified size.

init(count: Int)

Creates a new data buffer with the specified count of zeroed bytes.

