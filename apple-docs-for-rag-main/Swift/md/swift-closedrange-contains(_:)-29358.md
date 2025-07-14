

- Swift
- ClosedRange
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the given range is contained within this closed range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ other: Range) -> Bool
```

Available when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

## Parameters 

`other`  

A range to check for containment within this closed range.

## Return Value

`true` if `other` is empty or wholly contained within this closed range; otherwise, `false`.

## Discussion

The given range is contained within this closed range if the elements of the range are all contained within this closed range.

```
let range = 0...10
range.contains(5..

Additionally, passing any empty range as `other` results in the value `true`, even if the empty range’s bounds are outside the bounds of this closed range.

```
range.contains(3..

Complexity

O(1)

