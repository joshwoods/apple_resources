

- Swift
- RangeSet
-  isStrictSubset(of:) 

Instance Method

# isStrictSubset(of:)

Returns a Boolean value that indicates whether this range set is a strict subset of the given set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func isStrictSubset(of other: RangeSet) -> Bool
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`other`  

A range set to compare against.

## Return Value

`true` if this range set is a strict subset of `other`; otherwise, `false`.

