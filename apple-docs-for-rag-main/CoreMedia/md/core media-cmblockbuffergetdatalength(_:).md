

- Core Media
-  CMBlockBufferGetDataLength(\_:) 

Function

# CMBlockBufferGetDataLength(\_:)

Returns the total length of data that’s accessible by a block buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBlockBufferGetDataLength(_ theBuffer: CMBlockBuffer) -> Int
```

## Parameters 

`theBuffer`  

`CMBlockBuffer` to examine.

## Return Value

Returns the total data length available via this `CMBlockBuffer`, or zero if it is empty, `NULL` if invalid.

## Discussion

Obtains the total data length reachable via a `CMBlockBuffer`. This total is the sum of the `dataLengths` of the `CMBlockBuffer's` memoryBlocks and buffer references. Note that the `dataLengths` are the portions of those constituents that this `CMBlockBuffer` subscribes to. This `CMBlockBuffer` presents a contiguous range of offsets from zero to its `totalDataLength` as returned by this routine.

## See Also

### Inspecting a Block Buffer

func CMBlockBufferGetDataPointer(CMBlockBuffer, atOffset: Int, lengthAtOffsetOut: UnsafeMutablePointer&lt;Int>?, totalLengthOut: UnsafeMutablePointer&lt;Int>?, dataPointerOut: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>?) -> OSStatus

Gains access to the data represented by a block buffer.

func CMBlockBufferIsRangeContiguous(CMBlockBuffer, atOffset: Int, length: Int) -> Bool

Returns a Boolean value that indicates whether the specified range within a block buffer is contiguous.

func CMBlockBufferIsEmpty(CMBlockBuffer) -> Bool

Returns a Boolean value that indicates whether the buffer is empty.

