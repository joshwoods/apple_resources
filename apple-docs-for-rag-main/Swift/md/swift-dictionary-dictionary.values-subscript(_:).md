

- Swift
- Dictionary
- Dictionary.Values
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element at the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(position: Dictionary.Index) -> Dictionary.Values.Element { get set }
```

## Parameters 

`position`  

The position of the element to access. `position` must be a valid index of the collection that is not equal to the `endIndex` property.

## Overview

For example, you can replace an element of an array by using its subscript.

```
var streets = ["Adams", "Bryant", "Channing", "Douglas", "Evarts"]
streets[1] = "Butler"
print(streets[1])
// Prints "Butler"
```

You can subscript a collection with any valid index other than the collection’s end index. The end index refers to the position one past the last element of a collection, so it doesn’t correspond with an element.

Complexity

O(1)

