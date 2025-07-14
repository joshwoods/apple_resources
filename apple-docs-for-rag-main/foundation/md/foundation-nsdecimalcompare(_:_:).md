

- Foundation
-  NSDecimalCompare(\_:\_:) 

Function

# NSDecimalCompare(\_:\_:)

Compares two decimal values.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSDecimalCompare(
    _ leftOperand: UnsafePointer,
    _ rightOperand: UnsafePointer
) -> ComparisonResult
```

## Return Value

`NSOrderedDescending` if `leftOperand` is bigger than `rightOperand`; `NSOrderedAscending` if `rightOperand` is bigger than `leftOperand`; or `NSOrderedSame` if the two operands are equal.

## Discussion

For more information, see Number and Value Programming Topics.

## See Also

### Comparing decimals

func isEqual(to: Decimal) -> Bool

Indicates whether this decimal is equal to the specified one.

func isLess(than: Decimal) -> Bool

Indicates whether this decimal is less than the specified one.

func isLessThanOrEqualTo(Decimal) -> Bool

Indicates whether this decimal is less than or equal to the specified one.

func isTotallyOrdered(belowOrEqualTo: Decimal) -> Bool

Returns a Boolean value indicating whether this instance should precede the given value in an ascending sort.

