

- Swift
- UnsafeMutableBufferPointer
-  update(fromContentsOf:) 

Instance Method

# update(fromContentsOf:)

Updates the buffer’s initialized memory with every element of the source.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func update(fromContentsOf source: some Collection) -> UnsafeMutableBufferPointer.Index
```

## Parameters 

`source`  

A collection of elements to be used to update the buffer’s contents.

## Return Value

An index one past the index of the last element updated.

## Discussion

Prior to calling the `update(fromContentsOf:)` method on a buffer, the first `source.count` elements of the buffer’s memory must be initialized, or the buffer’s `Element` type must be a trivial type. The buffer must reference enough initialized memory to accommodate `source.count` elements.

The returned index is one past the index of the last element updated. If `source` contains no elements, the returned index is equal to the buffer’s `startIndex`. If `source` contains as many elements as the buffer can hold, the returned index is equal to the buffer’s `endIndex`.

Note

The memory regions referenced by `source` and this buffer may overlap.

Precondition

`self.count` \>= `source.count`

