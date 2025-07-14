

- Game Controller
- GCControllerDirectionPad
-  setValueForXAxis(\_:yAxis:) 

Instance Method

# setValueForXAxis(\_:yAxis:)

Sets the input values of a snapshot of a directional pad.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func setValueForXAxis(
    _ xAxis: Float,
    yAxis: Float
)
```

## Parameters 

`xAxis`  

A normalized value of the x-axis ranging from `-1` to `1`.

`yAxis`  

A normalized value for the y-axis ranging from `-1` to `1`.

## Discussion

This method does nothing if the associated controller isn’t a snapshot (its isSnapshot property is false`)`. Otherwise, this method sets the value of the direction pad’s buttons as well.

