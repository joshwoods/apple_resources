

- Core Media
-  CMBlockBufferIsEmpty(\_:) 

Function

# CMBlockBufferIsEmpty(\_:)

Returns a Boolean value that indicates whether the buffer is empty.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBlockBufferIsEmpty(_ theBuffer: CMBlockBuffer) -> Bool
```

## Parameters 

`theBuffer`  

`CMBlockBuffer` to examine. Must not be `NULL`.

## Return Value

False if the `CMBlockBuffer` is `NULL`.

## Discussion

Determines whether the given `CMBlockBuffer` is empty, i.e., devoid of any `memoryBlocks` or `CMBlockBuffer` references. Note that a `CMBlockBuffer` containing a not-yet allocated `memoryBlock` is not considered empty.

## See Also

### Inspecting a Block Buffer

func CMBlockBufferGetDataPointer(CMBlockBuffer, atOffset: Int, lengthAtOffsetOut: UnsafeMutablePointer&lt;Int>?, totalLengthOut: UnsafeMutablePointer&lt;Int>?, dataPointerOut: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>?) -> OSStatus

Gains access to the data represented by a block buffer.

func CMBlockBufferGetDataLength(CMBlockBuffer) -> Int

Returns the total length of data that’s accessible by a block buffer.

func CMBlockBufferIsRangeContiguous(CMBlockBuffer, atOffset: Int, length: Int) -> Bool

Returns a Boolean value that indicates whether the specified range within a block buffer is contiguous.

