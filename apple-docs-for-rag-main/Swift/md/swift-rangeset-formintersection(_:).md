

- Swift
- RangeSet
-  formIntersection(\_:) 

Instance Method

# formIntersection(\_:)

Removes the contents of this range set that aren’t also in the given range set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func formIntersection(_ other: RangeSet)
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`other`  

A range set to intersect with.

