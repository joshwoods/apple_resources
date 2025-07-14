

- Swift
- ClosedRange
-  overlaps(\_:) 

Instance Method

# overlaps(\_:)

Returns a Boolean value indicating whether this range and the given closed range contain an element in common.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func overlaps(_ other: ClosedRange) -> Bool
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`other`  

A range to check for elements in common.

## Return Value

`true` if this range and `other` have at least one element in common; otherwise, `false`.

## Discussion

This example shows two overlapping ranges:

```
let x: Range = 0...20
print(x.overlaps(10...1000))
// Prints "true"
```

## See Also

### Comparing Ranges

static func == (ClosedRange&lt;Bound>, ClosedRange&lt;Bound>) -> Bool

Returns a Boolean value indicating whether two ranges are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func overlaps(Range&lt;Bound>) -> Bool

Returns a Boolean value indicating whether this range and the given range contain an element in common.

