

- Swift
- RangeSet
-  remove(contentsOf:) 

Instance Method

# remove(contentsOf:)

Removes the given range from the range set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func remove(contentsOf range: Range)
```

## Parameters 

`range`  

The range to remove from the set.

## Discussion

Complexity

O(*n*), where *n* is the number of ranges in the range set.

