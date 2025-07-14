

- Foundation
- Data
-  replaceSubrange(\_:with:) 

Instance Method

# replaceSubrange(\_:with:)

Replaces a region of bytes in the data with new data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func replaceSubrange(
    _ subrange: Range,
    with data: Data
)
```

## Parameters 

`subrange`  

The range in the data to replace. If `subrange.lowerBound == data.count && subrange.count == 0` then this operation is an append.

`data`  

The replacement data.

## Discussion

This will resize the data if required, to fit the entire contents of `data`.

Precondition: The bounds of `subrange` must be valid indices of the collection.

## See Also

### Replacing a Range of Bytes

func replaceSubrange&lt;ByteCollection>(Range&lt;Data.Index>, with: ByteCollection)

Replaces a region of bytes in the data with new bytes from a collection.

func replaceSubrange&lt;SourceType>(Range&lt;Data.Index>, with: UnsafeBufferPointer&lt;SourceType>)

Replaces a region of bytes in the data with new bytes from a buffer.

func replaceSubrange(Range&lt;Data.Index>, with: UnsafeRawPointer, count: Int)

Replaces a region of bytes in the data with bytes from memory.

