

- Swift
- Array
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous subrange of the array’s elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(bounds: Range) -> ArraySlice { get set }
```

## Parameters 

`bounds`  

A range of integers. The bounds of the range must be valid indices of the array.

## Overview

The returned `ArraySlice` instance uses the same indices for the same elements as the original array. In particular, that slice, unlike an array, may have a nonzero `startIndex` and an `endIndex` that is not equal to `count`. Always use the slice’s `startIndex` and `endIndex` properties instead of assuming that its indices start or end at a particular value.

This example demonstrates getting a slice of an array of strings, finding the index of one of the strings in the slice, and then using that index in the original array.

```
let streets = ["Adams", "Bryant", "Channing", "Douglas", "Evarts"]
let streetsSlice = streets[2 ..

## See Also

### Accessing Elements

subscript(Int) -> Element

Accesses the element at the specified position.

var first: Self.Element?

The first element of the collection.

var last: Self.Element?

The last element of the collection.

subscript&lt;R>(R) -> Self.SubSequence

subscript&lt;R>(R) -> Self.SubSequence

Accesses the contiguous subrange of the collection’s elements specified by a range expression.

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

