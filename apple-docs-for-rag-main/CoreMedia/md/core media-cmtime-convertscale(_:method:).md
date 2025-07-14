

- Core Media
- CMTime
-  convertScale(\_:method:) 

Instance Method

# convertScale(\_:method:)

Converts the source time to a new timescale using the specified rounding method.

iOS 4.0+iPadOS 4.0+Mac CatalystmacOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func convertScale(
    _ newTimescale: Int32,
    method: CMTimeRoundingMethod
) -> CMTime
```

## Parameters 

`newTimescale`  

The timescale to use for the converted time.

`method`  

The rounding method to apply.

## Return Value

A converted time value.

## See Also

### Changing the Timescale

enum CMTimeRoundingMethod

An enumeration of rounding methods to use when performing time calculations.

