

- Swift
- Slice
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous subrange of the collection’s elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(bounds: Range) -> Slice { get set }
```

Available when `SubSequence` is `Slice`.

## Parameters 

`bounds`  

A range of the collection’s indices. The bounds of the range must be valid indices of the collection.

## Overview

The accessed slice uses the same indices for the same elements as the original collection. Always use the slice’s `startIndex` property instead of assuming that its indices start at a particular value.

This example demonstrates getting a slice of an array of strings, finding the index of one of the strings in the slice, and then using that index in the original array.

```
var streets = ["Adams", "Bryant", "Channing", "Douglas", "Evarts"]
let streetsSlice = streets[2 ..

Complexity

O(1)

