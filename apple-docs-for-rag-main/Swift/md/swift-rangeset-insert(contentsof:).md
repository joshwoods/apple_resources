

- Swift
- RangeSet
-  insert(contentsOf:) 

Instance Method

# insert(contentsOf:)

Inserts the given range into the range set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func insert(contentsOf range: Range)
```

## Parameters 

`range`  

The range to insert into the set.

## Discussion

Complexity

O(*n*), where *n* is the number of ranges in the range set.

