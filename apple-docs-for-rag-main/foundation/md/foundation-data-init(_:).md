

- Foundation
- Data
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance of a collection containing the elements of a sequence.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ elements: S) where S : Sequence, Self.Element == S.Element
```

## Parameters 

`elements`  

The sequence of elements for the new collection.

## See Also

### Creating Populated Data

init()

Creates an empty data buffer.

init&lt;SourceType>(buffer: UnsafeBufferPointer&lt;SourceType>)

Creates a data buffer with copied memory content using a buffer pointer.

init&lt;SourceType>(buffer: UnsafeMutableBufferPointer&lt;SourceType>)

Creates a data buffer with copied memory content using a mutable buffer pointer.

init(bytes: UnsafeRawPointer, count: Int)

Creates data with copied memory content.

init(bytesNoCopy: UnsafeMutableRawPointer, count: Int, deallocator: Data.Deallocator)

Creates a data buffer with memory content without copying the bytes.

init(capacity: Int)

Creates an empty data buffer of a specified size.

init(count: Int)

Creates a new data buffer with the specified count of zeroed bytes.

