

- Foundation
- NSDecimalNumberBehaviors
-  scale() 

Instance Method

# scale()

Returns the number of digits allowed after the decimal separator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func scale() -> Int16
```

**Required**

## Return Value

The number of digits allowed after the decimal separator.

## Discussion

This method limits the precision of the values returned by `NSDecimalNumber`’s `decimalNumberBy...` methods. If scale() returns a negative value, it affects the digits before the decimal separator as well. If scale() returns `NSDecimalNoScale`, the number of digits is unlimited.

Assuming that roundingMode() returns `NSRoundPlain`, different values of scale() have the following effects on the number 123.456:

| Scale              | Return Value |
|--------------------|--------------|
| `NSDecimalNoScale` | 123.456      |
| 2                  | 123.45       |
| 0                  | 123          |
| –2                 | 100          |

## See Also

### Rounding

func roundingMode() -> NSDecimalNumber.RoundingMode

Returns the way that `NSDecimalNumber`’s `decimalNumberBy...` methods round their return values.

**Required**

