

- Foundation
- Data
-  copyBytes(to:count:) 

Instance Method

# copyBytes(to:count:)

Copies the contents of the data to memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func copyBytes(
    to pointer: UnsafeMutablePointer,
    count: Int
)
```

## Parameters 

`pointer`  

A pointer to the buffer you wish to copy the bytes into.

`count`  

The number of bytes to copy.

## Discussion

Warning

This method does not verify that the contents at pointer have enough space to hold `count` bytes.

## See Also

### Accessing Underlying Memory

func withUnsafeBytes&lt;ResultType, ContentType>((UnsafePointer&lt;ContentType>) throws -> ResultType) rethrows -> ResultType

Accesses the raw bytes in the data’s buffer.

func withUnsafeMutableBytes&lt;ResultType, ContentType>((UnsafeMutablePointer&lt;ContentType>) throws -> ResultType) rethrows -> ResultType

Mutates the raw bytes in the data’s buffer.

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, from: Range&lt;Data.Index>)

Copies a subset of the contents of the data to memory.

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: Range&lt;Data.Index>?) -> Int

Copies the bytes in a range from the data into a buffer.

