

- Game Controller
- GCControllerTouchpad
-  setValueForXAxis(\_:yAxis:touchDown:buttonValue:) 

Instance Method

# setValueForXAxis(\_:yAxis:touchDown:buttonValue:)

Sets the input values of a snapshot of a touchpad.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func setValueForXAxis(
    _ xAxis: Float,
    yAxis: Float,
    touchDown: Bool,
    buttonValue: Float
)
```

## Parameters 

`xAxis`  

A normalized value of the x-axis ranging from `-1` to `1`.

`yAxis`  

A normalized value of the y-axis ranging from `-1` to `1`.

`touchDown`  

A Boolean value that indicates whether the user starts touching the surface. If true, the user is touching the surface; otherwise, the user isn’t.

`buttonValue`  

A normalized number between `0.0` (minimum) and `1.0` (maximum) that represents the level of pressure the user applies to the button.

## Discussion

This method does nothing if the associated controller isn’t a snapshot (its isSnapshot property is false`)`.

