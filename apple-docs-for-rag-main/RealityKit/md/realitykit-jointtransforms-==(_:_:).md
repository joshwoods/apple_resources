

- RealityKit
- JointTransforms
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two collections of joints are equal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
static func == (lhs: JointTransforms, rhs: JointTransforms) -> Bool
```

## Parameters 

`lhs`  

The collection of joints on the left side of the operator.

`rhs`  

The collection of joints on the right side of the operator.

## Return Value

Returns `true` if the two collections of joints are equal. Otherwise, returns `false`.

## See Also

### Comparing joint transforms

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func compare&lt;Comparator>(Comparator.Compared, Comparator.Compared) -> ComparisonResult

If `lhs` is ordered before `rhs` in the ordering described by the given sequence of `SortComparator`s

