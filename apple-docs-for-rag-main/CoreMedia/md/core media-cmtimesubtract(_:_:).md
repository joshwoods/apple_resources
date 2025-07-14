

- Core Media
-  CMTimeSubtract(\_:\_:) 

Function

# CMTimeSubtract(\_:\_:)

Returns the difference between two times.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeSubtract(
    _ lhs: CMTime,
    _ rhs: CMTime
) -> CMTime
```

## Parameters 

`lhs`  

A time value.

`rhs`  

A time value to subtract from the minuend.

## Return Value

A time value that represents the result of the operation.

## Discussion

If the operands have the same timescale, the timescale of the result is the same as the operands’ timescale. If the operands have different timescales, the timescale of the result is the least common multiple of the operands’ timescales. If that LCM timescale is greater than kCMTimeMaxTimescale, the result timescale is kCMTimeMaxTimescale, and the system applies the default rounding when it converts the result to this timescale.

If the value of the result overflows, the system repeatedly halves its timescale until it no longer overflows, and uses the default rounding to convert the result to this timescale. If the result’s value still overflows when its timescale is `1`, the system sets the result’s timescale to positive or negative infinity, depending on the direction of the overflow. If any rounding occurs, or if either operand has its hasBeenRounded flag set, the system sets the result’s hasBeenRounded flag.

If either operand is invalid, the result is invalid. If the operands are valid, but one is infinite, the result is infinite. If the operands are valid, and both are infinite, the results are as follows:

- +infinity - +infinity == invalid

- -infinity - -infinity == invalid

- +infinity - -infinity == +infinity

- -infinity + +infinity == invalid

If the operands are valid, not infinite, and either or both is indefinite, the result is indefinite.

If the two operands are numeric, but have different nonzero epochs, the result is invalid. If both have the same nonzero epoch, the result is epoch zero. You can’t add or subtract times that have different epochs, because the epoch length is unknown. The system considers times in epoch zero to be durations, so you can add them to times in other epochs. You can compare times in different epochs, however, because numerically greater epochs always occur after numerically lesser epochs.

## See Also

### Performing Time Calculations

func CMTimeAdd(CMTime, CMTime) -> CMTime

Returns the sum of two times.

func CMTimeMultiply(CMTime, multiplier: Int32) -> CMTime

Returns the result of multiplying a time by an integer multiplier.

func CMTimeMultiplyByFloat64(CMTime, multiplier: Float64) -> CMTime

Returns the result of multiplying a time by a floating-point multiplier.

func CMTimeMultiplyByRatio(CMTime, multiplier: Int32, divisor: Int32) -> CMTime

Returns the result of multiplying a time by an integer multiplier, and then dividing the result by the divisor.

