

- Swift
- RangeSet
-  symmetricDifference(\_:) 

Instance Method

# symmetricDifference(\_:)

Returns a new range set representing the values in this range set or the given range set, but not both.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func symmetricDifference(_ other: RangeSet) -> RangeSet
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`other`  

The range set to find a symmetric difference with.

## Return Value

A new range set.

