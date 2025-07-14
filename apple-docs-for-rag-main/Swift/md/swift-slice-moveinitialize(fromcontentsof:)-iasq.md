

- Swift
- Slice
-  moveInitialize(fromContentsOf:) 

Instance Method

# moveInitialize(fromContentsOf:)

Moves every element of an initialized source buffer slice into the uninitialized memory referenced by this buffer slice, leaving the source memory uninitialized and this buffer slice’s memory initialized.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func moveInitialize(fromContentsOf source: Slice>) -> Slice.Index where Base == UnsafeMutableBufferPointer
```

Available when `Base` conforms to `Collection`.

## Parameters 

`source`  

A buffer slice containing the values to copy. The memory region underlying `source` must be initialized.

## Return Value

The index one past the last element of the buffer slice initialized by this function.

## Discussion

Prior to calling the `moveInitialize(fromContentsOf:)` method on a buffer slice, the memory it references must be uninitialized, or its `Element` type must be a trivial type. After the call, the memory referenced by the buffer slice up to, but not including, the returned index is initialized. The memory referenced by `source` is uninitialized after the function returns. The buffer slice must reference enough memory to accommodate `source.count` elements.

The returned index is the position of the next uninitialized element in the buffer slice, one past the index of the last element written. If `source` contains no elements, the returned index is equal to the slice’s `startIndex`. If `source` contains as many elements as the slice can hold, the returned index is equal to the slice’s `endIndex`.

Note

The memory regions referenced by `source` and this buffer slice may overlap.

Precondition

`self.count` \>= `source.count`

