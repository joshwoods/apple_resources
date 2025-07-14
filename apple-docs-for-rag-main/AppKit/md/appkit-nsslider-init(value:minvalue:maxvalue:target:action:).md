

- AppKit
- NSSlider
-  init(value:minValue:maxValue:target:action:) 

Initializer

# init(value:minValue:maxValue:target:action:)

Creates a continuous horizontal slider that represents values over the specified range.

macOS 10.12+

``` source
@MainActor
convenience init(
    value: Double,
    minValue: Double,
    maxValue: Double,
    target: Any?,
    action: Selector?
)
```

## Parameters 

`value`  

The initial value displayed by the control.

`minValue`  

The minimum value that the control can represent.

`maxValue`  

The maximum value that the control can represent.

`target`  

The target object that receives action messages from the control.

`action`  

The action message sent by the control.

## Return Value

An initialized slider control.

## See Also

### Creating Sliders

convenience init(target: Any?, action: Selector?)

Creates a continuous horizontal slider whose values range from `0.0` to `1.0`.

