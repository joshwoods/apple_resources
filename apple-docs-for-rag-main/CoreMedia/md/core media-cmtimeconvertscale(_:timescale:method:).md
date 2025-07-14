

- Core Media
-  CMTimeConvertScale(\_:timescale:method:) 

Function

# CMTimeConvertScale(\_:timescale:method:)

Converts the source time to a new timescale using the specified rounding method.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeConvertScale(
    _ time: CMTime,
    timescale newTimescale: Int32,
    method: CMTimeRoundingMethod
) -> CMTime
```

## Parameters 

`time`  

The time to convert.

`newTimescale`  

The timescale to use for the converted time.

`method`  

The rounding method to apply.

## Return Value

A time structure that represents the time in a new timescale.

## Discussion

If this operation needs to round the value, it sets the resulting time’s hasBeenRounded flag. If the source time is nonnumeric (infinite, indefinite, or invalid), the result is also nonnumeric.

## See Also

### Changing the Timescale

enum CMTimeRoundingMethod

An enumeration of rounding methods to use when performing time calculations.

