

- Game Controller
-  GCControllerDirectionPadValueChangedHandler 

Type Alias

# GCControllerDirectionPadValueChangedHandler

The signature for the block that executes when either axis changes values.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
typealias GCControllerDirectionPadValueChangedHandler = (GCControllerDirectionPad, Float, Float) -> Void
```

## Parameters 

`dpad`  

The directional pad element that changed.

`xValue`  

A normalized value of the x-axis ranging from `-1` to `1`.

`yValue`  

A normalized value of the y-axis ranging from `-1` to `1`.

## See Also

### Getting change information

var valueChangedHandler: GCControllerDirectionPadValueChangedHandler?

The block that the directional pad calls when the user changes its values.

