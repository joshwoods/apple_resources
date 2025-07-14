

- Core Media
-  CMTimeMultiplyByRatio(\_:multiplier:divisor:) 

Function

# CMTimeMultiplyByRatio(\_:multiplier:divisor:)

Returns the result of multiplying a time by an integer multiplier, and then dividing the result by the divisor.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeMultiplyByRatio(
    _ time: CMTime,
    multiplier: Int32,
    divisor: Int32
) -> CMTime
```

## Parameters 

`time`  

A time value to multiple by a ratio.

`multiplier`  

The value by which to multiply.

`divisor`  

The value by which to divide.

## Return Value

A value equal to `(time * multiplier) / divisor`.

## Discussion

This method preserves the exact rational value, unless it causes an overflow. If an overflow occurs, the system chooses a new timescale to minimize the rounding error and applies the default rounding method when converting the result to this timescale. If the result’s value still overflows when its timescale is `1`, the system sets the result to positive or negative infinity, depending on the direction of the overflow.

If rounding occurs for any reason, the system sets the result’s hasBeenRounded flag. It also sets this flag if the time argument has its hasBeenRounded flag set.

If the time value or timescale is zero, the result is invalid. If only the timescale is zero, the result is positive or negative infinity, depending on the signs of the other arguments.

If time is invalid, the result is invalid. If time is infinite, the result is similarly infinite. If time is indefinite, the result is indefinite.

## See Also

### Performing Time Calculations

func CMTimeAdd(CMTime, CMTime) -> CMTime

Returns the sum of two times.

func CMTimeSubtract(CMTime, CMTime) -> CMTime

Returns the difference between two times.

func CMTimeMultiply(CMTime, multiplier: Int32) -> CMTime

Returns the result of multiplying a time by an integer multiplier.

func CMTimeMultiplyByFloat64(CMTime, multiplier: Float64) -> CMTime

Returns the result of multiplying a time by a floating-point multiplier.

