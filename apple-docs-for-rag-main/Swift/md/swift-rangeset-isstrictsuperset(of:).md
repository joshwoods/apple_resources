

- Swift
- RangeSet
-  isStrictSuperset(of:) 

Instance Method

# isStrictSuperset(of:)

Returns a Boolean value that indicates whether this range set is a strict superset of the given set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func isStrictSuperset(of other: RangeSet) -> Bool
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`other`  

A range set to compare against.

## Return Value

`true` if this range set is a strict superset of `other`; otherwise, `false`.

