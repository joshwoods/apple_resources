

- System
- FilePath
- FilePath.ComponentView
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Creates a new collection by concatenating the elements of two collections.

SystemSwiftiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func + (lhs: Self, rhs: Other) -> Self where Other : RangeReplaceableCollection, Self.Element == Other.Element
```

## Parameters 

`lhs`  

A range-replaceable collection.

`rhs`  

Another range-replaceable collection.

## Discussion

The two arguments must have the same `Element` type. For example, you can concatenate the elements of two integer arrays.

```
let lowerNumbers = [1, 2, 3, 4]
let higherNumbers: ContiguousArray = [5, 6, 7, 8, 9, 10]
let allNumbers = lowerNumbers + higherNumbers
print(allNumbers)
// Prints "[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]"
```

The resulting collection has the type of the argument on the left-hand side. In the example above, `moreNumbers` has the same type as `numbers`, which is `[Int]`.

