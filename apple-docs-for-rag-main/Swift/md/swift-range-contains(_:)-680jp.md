

- Swift
- Range
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the given closed range is contained within this range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ other: ClosedRange) -> Bool
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`other`  

A closed range to check for containment within this range.

## Return Value

`true` if `other` is wholly contained within this range; otherwise, `false`.

## Discussion

The given closed range is contained within this range if its bounds are contained within this range. If this range is empty, it cannot contain a closed range, since closed ranges by definition contain their boundaries.

```
let range = 0..

Complexity

O(1)

