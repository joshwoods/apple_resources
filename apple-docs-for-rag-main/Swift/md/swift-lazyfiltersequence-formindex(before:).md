

- Swift
- LazyFilterSequence
-  formIndex(before:) 

Instance Method

# formIndex(before:)

Replaces the given index with its predecessor.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func formIndex(before i: inout LazyFilterSequence.Index)
```

Available when `Base` conforms to `BidirectionalCollection`.

## Parameters 

`i`  

A valid index of the collection. `i` must be greater than `startIndex`.

