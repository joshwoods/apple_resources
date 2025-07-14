

- Swift
- UnsafeMutableBufferPointer
-  update(from:) 

Instance Method

# update(from:)

Updates the buffer’s initialized memory with the given elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func update(from source: S) -> (unwritten: S.Iterator, index: UnsafeMutableBufferPointer.Index) where Element == S.Element, S : Sequence
```

## Parameters 

`source`  

A sequence of elements to be used to update the buffer’s contents.

## Return Value

An iterator to any elements of `source` that didn’t fit in the buffer, and the index one past the last updated element in the buffer.

## Discussion

The buffer’s memory must be initialized or its `Element` type must be a trivial type.

