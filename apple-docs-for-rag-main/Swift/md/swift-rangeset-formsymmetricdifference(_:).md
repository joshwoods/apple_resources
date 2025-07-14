

- Swift
- RangeSet
-  formSymmetricDifference(\_:) 

Instance Method

# formSymmetricDifference(\_:)

Removes the contents of this range set that are also in the given set and adds the contents of the given set that are not already in this range set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func formSymmetricDifference(_ other: RangeSet)
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`other`  

A range set to perform a symmetric difference against.

