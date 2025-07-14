

- Swift
- ArraySlice
-  moveSubranges(\_:to:) 

Instance Method

# moveSubranges(\_:to:)

Moves the elements in the given subranges to just before the element at the specified index.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@discardableResult
mutating func moveSubranges(
    _ subranges: RangeSet,
    to insertionPoint: Self.Index
) -> Range
```

## Parameters 

`subranges`  

The subranges of the elements to move.

`insertionPoint`  

The index to use as the destination of the elements.

## Return Value

The new bounds of the moved elements.

## Discussion

This example finds all the uppercase letters in the array and then moves them to between `"i"` and `"j"`.

```
var letters = Array("ABCdeFGhijkLMNOp")
let uppercaseRanges = letters.subranges(where: { $0.isUppercase })
let rangeOfUppercase = letters.moveSubranges(uppercaseRanges, to: 10)
// String(letters) == "dehiABCFGLMNOjkp"
// rangeOfUppercase == 4..

Complexity

O(*n* log *n*) where *n* is the length of the collection.

