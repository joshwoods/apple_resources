

- Game Controller
-  GCControllerAxisValueChangedHandler 

Type Alias

# GCControllerAxisValueChangedHandler

The signature for the block that executes when the user changes the axis value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
typealias GCControllerAxisValueChangedHandler = (GCControllerAxisInput, Float) -> Void
```

## Parameters 

`axis`  

The axis that the user changed.

`value`  

A normalized value for the axis ranging from `-1` to `1`.

## See Also

### Getting change information

var valueChangedHandler: GCControllerAxisValueChangedHandler?

The block that the element calls when the user changes the axis value.

