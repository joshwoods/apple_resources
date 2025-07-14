

- Foundation
- Decimal
-  isTotallyOrdered(belowOrEqualTo:) 

Instance Method

# isTotallyOrdered(belowOrEqualTo:)

Returns a Boolean value indicating whether this instance should precede the given value in an ascending sort.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isTotallyOrdered(belowOrEqualTo other: Decimal) -> Bool
```

## See Also

### Comparing decimals

func isEqual(to: Decimal) -> Bool

Indicates whether this decimal is equal to the specified one.

func isLess(than: Decimal) -> Bool

Indicates whether this decimal is less than the specified one.

func isLessThanOrEqualTo(Decimal) -> Bool

Indicates whether this decimal is less than or equal to the specified one.

func NSDecimalCompare(UnsafePointer&lt;Decimal>, UnsafePointer&lt;Decimal>) -> ComparisonResult

Compares two decimal values.

