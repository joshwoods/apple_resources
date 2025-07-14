

- Foundation
- Data
-  replaceSubrange(\_:with:) 

Instance Method

# replaceSubrange(\_:with:)

Replaces a region of bytes in the data with new bytes from a buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func replaceSubrange(
    _ subrange: Range,
    with buffer: UnsafeBufferPointer
)
```

## Parameters 

`subrange`  

The range in the data to replace.

`buffer`  

The replacement bytes.

## Discussion

This will resize the data if required, to fit the entire contents of `buffer`.

Precondition: The bounds of `subrange` must be valid indices of the collection.

## See Also

### Replacing a Range of Bytes

func replaceSubrange(Range&lt;Data.Index>, with: Data)

Replaces a region of bytes in the data with new data.

func replaceSubrange&lt;ByteCollection>(Range&lt;Data.Index>, with: ByteCollection)

Replaces a region of bytes in the data with new bytes from a collection.

func replaceSubrange(Range&lt;Data.Index>, with: UnsafeRawPointer, count: Int)

Replaces a region of bytes in the data with bytes from memory.

