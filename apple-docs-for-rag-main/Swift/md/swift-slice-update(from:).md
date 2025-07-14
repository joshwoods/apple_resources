

- Swift
- Slice
-  update(from:) 

Instance Method

# update(from:)

Updates the buffer slice’s initialized memory with the given elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func update(from source: S) -> (unwritten: S.Iterator, index: Slice.Index) where Base == UnsafeMutableBufferPointer, S : Sequence
```

Available when `Base` conforms to `Collection`.

## Parameters 

`source`  

A sequence of elements to be used to update the contents of the buffer slice.

## Return Value

An iterator to any elements of `source` that didn’t fit in the buffer slice, and the index one past the last updated element.

## Discussion

The buffer slice’s memory must be initialized or its `Element` type must be a trivial type.

