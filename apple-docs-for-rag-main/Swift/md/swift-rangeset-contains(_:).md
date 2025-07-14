

- Swift
- RangeSet
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the given value is contained by the ranges in the range set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func contains(_ value: Bound) -> Bool
```

## Parameters 

`value`  

The value to look for in the range set.

## Return Value

`true` if `value` is contained by a range in the range set; otherwise, `false`.

## Discussion

Complexity

O(log *n*), where *n* is the number of ranges in the range set.

