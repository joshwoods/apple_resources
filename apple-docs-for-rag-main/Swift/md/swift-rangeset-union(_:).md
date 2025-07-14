

- Swift
- RangeSet
-  union(\_:) 

Instance Method

# union(\_:)

Returns a new range set containing the contents of both this set and the given set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func union(_ other: RangeSet) -> RangeSet
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`other`  

The range set to merge with this one.

## Return Value

A new range set.

