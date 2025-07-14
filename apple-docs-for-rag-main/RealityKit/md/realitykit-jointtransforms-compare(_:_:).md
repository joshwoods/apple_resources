

- RealityKit
- JointTransforms
-  compare(\_:\_:) 

Instance Method

# compare(\_:\_:)

If `lhs` is ordered before `rhs` in the ordering described by the given sequence of `SortComparator`s

RealityKitSwiftiOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func compare(
    _ lhs: Comparator.Compared,
    _ rhs: Comparator.Compared
) -> ComparisonResult where Comparator : SortComparator, Comparator == Self.Element
```

## Discussion

The first element of the sequence of comparators specifies the primary comparator to be used in sorting the sequence’s elements. Any subsequent comparators are used to further refine the order of elements with equal values.

## See Also

### Comparing joint transforms

static func == (JointTransforms, JointTransforms) -> Bool

Returns a Boolean value that indicates whether two collections of joints are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

