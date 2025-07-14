

- Swift
- RangeSet
-  formUnion(\_:) 

Instance Method

# formUnion(\_:)

Adds the contents of the given range set to this range set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func formUnion(_ other: RangeSet)
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`other`  

A range set to merge with this one.

## Discussion

Complexity

O(*m* + *n*), where *m* and *n* are the number of ranges in this and the other range set.

