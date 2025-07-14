

- Swift
- Collection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element at the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(position: Self.Index) -> Self.Element { get }
```

**Required** Default implementations provided.

## Parameters 

`position`  

The position of the element to access. `position` must be a valid index of the collection that is not equal to the `endIndex` property.

## Overview

The following example accesses an element of an array through its subscript to print its value:

```
var streets = ["Adams", "Bryant", "Channing", "Douglas", "Evarts"]
print(streets[1])
// Prints "Bryant"
```

You can subscript a collection with any valid index other than the collection’s end index. The end index refers to the position one past the last element of a collection, so it doesn’t correspond with an element.

Complexity

O(1)

## Default Implementations

### Collection Implementations

subscript(RangeSet&lt;Self.Index>) -> DiscontiguousSlice&lt;Self>

Accesses a view of this collection with the elements at the given indices.

subscript(Range&lt;Self.Index>) -> Slice&lt;Self>

Accesses a contiguous subrange of the collection’s elements.

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

subscript&lt;R>(R) -> Self.SubSequence

Accesses the contiguous subrange of the collection’s elements specified by a range expression.

### MutableCollection Implementations

subscript(Range&lt;Self.Index>) -> Slice&lt;Self>

Accesses a contiguous subrange of the collection’s elements.

subscript&lt;R>(R) -> Self.SubSequence

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

