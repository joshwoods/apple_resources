

- Core Media
- CMTime
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Returns a new time that represents the sum of two times.

iOS 4.0+iPadOS 4.0+Mac CatalystmacOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
static func + (addend1: CMTime, addend2: CMTime) -> CMTime
```

## Parameters 

`addend1`  

The first time value.

`addend2`  

The second time value.

## Return Value

A time value that represents the result of the operation.

## Discussion

If both operands have the same timescale, the timescale of the result is the same. If the operands have different timescales, the timescale of the result is the least common multiple of the operands’ timescales. If that value is greater than kCMTimeMaxTimescale, the system sets the timescale to kCMTimeMaxTimescale and uses the default rounding method to convert the result to this timescale.

If the value of the result overflows, the system repeatedly halves its timescale until it no longer overflows, and uses the default rounding to convert the result to this timescale. If the result’s value still overflows when its timescale is `1`, the system sets the result’s timescale to positive or negative infinity, depending on the direction of the overflow. If any rounding occurs, or if either operand has its hasBeenRounded flag set, the system sets the result’s hasBeenRounded flag.

If either of the operands is invalid, the result is invalid.

If the operands are valid, but one is infinite, the result is infinite. If the operands are valid, and both are infinite, the results are as follows:

- +infinity + +infinity == +infinity

- -infinity + -infinity == -infinity

- +infinity + -infinity == invalid

- -infinity + +infinity == invalid

If the operands are valid, not infinite, and either or both is indefinite, the result is indefinite.

If the two operands are numeric, but have different nonzero epochs, the result is invalid. If both have the same nonzero epoch, the result is epoch zero. You can’t add or subtract times that have different epochs, because the epoch length is unknown. The system considers times in epoch zero to be durations, so you can add them to times in other epochs. You can compare times in different epochs, however, because numerically greater epochs always occur after numerically lesser epochs.

## See Also

### Performing Time Calcualtions

static func - (CMTime, CMTime) -> CMTime

Returns a new time that represents the difference between two times.

