

- Swift
- Slice
-  moveUpdate(fromContentsOf:) 

Instance Method

# moveUpdate(fromContentsOf:)

Updates this buffer slice’s initialized memory initialized memory by moving every element from the source buffer slice, leaving the source memory uninitialized.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func moveUpdate(fromContentsOf source: Slice>) -> Slice.Index where Base == UnsafeMutableBufferPointer
```

Available when `Base` conforms to `Collection`.

## Parameters 

`source`  

A buffer slice containing the values to move. The memory region underlying `source` must be initialized.

## Return Value

An index one past the index of the last element updated.

## Discussion

The region of memory starting at the beginning of this buffer slice and covering `source.count` instances of its `Element` type must be initialized, or its `Element` type must be a trivial type. After calling `moveUpdate(fromContentsOf:)`, the region of memory underlying `source` is uninitialized. The buffer slice must reference enough initialized memory to accommodate `source.count` elements.

The returned index is one past the index of the last element updated. If `source` contains no elements, the returned index is equal to the buffer’s `startIndex`. If `source` contains as many elements as the buffer slice can hold, the returned index is equal to the slice’s `endIndex`.

Note

The memory regions referenced by `source` and this buffer slice must not overlap.

Precondition

`self.count` \>= `source.count`

