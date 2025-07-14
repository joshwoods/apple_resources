

- Core Media
-  CMBlockBufferIsRangeContiguous(\_:atOffset:length:) 

Function

# CMBlockBufferIsRangeContiguous(\_:atOffset:length:)

Returns a Boolean value that indicates whether the specified range within a block buffer is contiguous.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBlockBufferIsRangeContiguous(
    _ theBuffer: CMBlockBuffer,
    atOffset offset: Int,
    length: Int
) -> Bool
```

## Parameters 

`theBuffer`  

`CMBlockBuffer` to examine. Must not be `NULL`.

`offset`  

Offset within the buffer’s offset range.

`length`  

Desired number of bytes to access at offset. If zero, the number of bytes available at offset (dataLength – offset), contiguous or not, is used.

## Return Value

Returns true if the specified range is contiguous within the `CMBlockBuffer`, false otherwise. Also returns false if the `CMBlockBuffer` is `NULL` or empty.

## Discussion

Determines whether the specified range within the given `CMBlockBuffer` is contiguous. If `CMBlockBufferGetDataPointer`() were called with the same parameters, the returned pointer would address the desired number of bytes.

## See Also

### Inspecting a Block Buffer

func CMBlockBufferGetDataPointer(CMBlockBuffer, atOffset: Int, lengthAtOffsetOut: UnsafeMutablePointer&lt;Int>?, totalLengthOut: UnsafeMutablePointer&lt;Int>?, dataPointerOut: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>?) -> OSStatus

Gains access to the data represented by a block buffer.

func CMBlockBufferGetDataLength(CMBlockBuffer) -> Int

Returns the total length of data that’s accessible by a block buffer.

func CMBlockBufferIsEmpty(CMBlockBuffer) -> Bool

Returns a Boolean value that indicates whether the buffer is empty.

