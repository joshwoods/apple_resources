

- Foundation
- Data
-  replaceSubrange(\_:with:count:) 

Instance Method

# replaceSubrange(\_:with:count:)

Replaces a region of bytes in the data with bytes from memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func replaceSubrange(
    _ subrange: Range,
    with bytes: UnsafeRawPointer,
    count cnt: Int
)
```

## See Also

### Replacing a Range of Bytes

func replaceSubrange(Range&lt;Data.Index>, with: Data)

Replaces a region of bytes in the data with new data.

func replaceSubrange&lt;ByteCollection>(Range&lt;Data.Index>, with: ByteCollection)

Replaces a region of bytes in the data with new bytes from a collection.

func replaceSubrange&lt;SourceType>(Range&lt;Data.Index>, with: UnsafeBufferPointer&lt;SourceType>)

Replaces a region of bytes in the data with new bytes from a buffer.

