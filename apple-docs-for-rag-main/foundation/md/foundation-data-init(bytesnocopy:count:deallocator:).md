

- Foundation
- Data
-  init(bytesNoCopy:count:deallocator:) 

Initializer

# init(bytesNoCopy:count:deallocator:)

Creates a data buffer with memory content without copying the bytes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    bytesNoCopy bytes: UnsafeMutableRawPointer,
    count: Int,
    deallocator: Data.Deallocator
)
```

## Parameters 

`bytes`  

A pointer to the bytes.

`count`  

The size of the bytes.

`deallocator`  

Specifies the mechanism to free the indicated buffer, or `.none`.

## Discussion

If the result is mutated and is not a unique reference, then the `Data` will still follow copy-on-write semantics. In this case, the copy will use its own deallocator. Therefore, it is usually best to only use this initializer when you either enforce immutability with `let` or ensure that no other references to the underlying data are formed.

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

init(bytes: UnsafeRawPointer, count: Int)

Creates data with copied memory content.

init(capacity: Int)

Creates an empty data buffer of a specified size.

init(count: Int)

Creates a new data buffer with the specified count of zeroed bytes.

