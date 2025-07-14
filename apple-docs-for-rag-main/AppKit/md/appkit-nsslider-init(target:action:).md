

- AppKit
- NSSlider
-  init(target:action:) 

Initializer

# init(target:action:)

Creates a continuous horizontal slider whose values range from `0.0` to `1.0`.

macOS 10.12+

``` source
@MainActor
convenience init(
    target: Any?,
    action: Selector?
)
```

## Parameters 

`target`  

The target object that receives action messages from the control.

`action`  

The action message sent by the control.

## Return Value

An initialized slider control.

## See Also

### Related Documentation

Slider Programming Topics

### Creating Sliders

convenience init(value: Double, minValue: Double, maxValue: Double, target: Any?, action: Selector?)

Creates a continuous horizontal slider that represents values over the specified range.

