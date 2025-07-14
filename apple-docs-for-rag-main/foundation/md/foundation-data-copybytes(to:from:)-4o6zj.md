

- Foundation
- Data
-  copyBytes(to:from:) 

Instance Method

# copyBytes(to:from:)

Copies the bytes in a range from the data into a buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func copyBytes(
    to buffer: UnsafeMutableBufferPointer,
    from range: Range? = nil
) -> Int
```

## Parameters 

`buffer`  

A buffer to copy the data into.

`range`  

A range in the data to copy into the buffer. If the range is empty, this function will return 0 without copying anything. If the range is nil, as much data as will fit into `buffer` is copied.

## Return Value

Number of bytes copied into the destination buffer.

## Discussion

If the count of the range is greater than `MemoryLayout.stride * buffer.count` then only the first `N` bytes will be copied into the buffer.Precondition: The range must be within the bounds of the data. Otherwise `fatalError` is called.

## See Also

### Accessing Underlying Memory

func withUnsafeBytes&lt;ResultType, ContentType>((UnsafePointer&lt;ContentType>) throws -> ResultType) rethrows -> ResultType

Accesses the raw bytes in the data’s buffer.

func withUnsafeMutableBytes&lt;ResultType, ContentType>((UnsafeMutablePointer&lt;ContentType>) throws -> ResultType) rethrows -> ResultType

Mutates the raw bytes in the data’s buffer.

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, count: Int)

Copies the contents of the data to memory.

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, from: Range&lt;Data.Index>)

Copies a subset of the contents of the data to memory.

