

- Game Controller
- GCControllerButtonInput
-  setValue(\_:) 

Instance Method

# setValue(\_:)

Sets the pressure value of a snapshot of a button.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func setValue(_ value: Float)
```

## Parameters 

`value`  

A normalized number between `0.0` (minimum pressure) and `1.0` (maximum pressure).

## Discussion

This method does nothing if the associated controller isn’t a snapshot (its isSnapshot property is false`)`.

