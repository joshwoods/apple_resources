

- Swift
- RangeSet
- RangeSet.Ranges
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element at the specified position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
subscript(i: RangeSet.Ranges.Index) -> RangeSet.Ranges.Element { get }
```

Available when `Bound` conforms to `Comparable`.

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

