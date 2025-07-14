

- RealityKit
- PhysicsJoints
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element at the specified position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
subscript(index: Int) -> any PhysicsJoint { get set }
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

