

- Game Controller
-  GCMicroGamepadValueChangedHandler 

Type Alias

# GCMicroGamepadValueChangedHandler

Signature for the block that this profile calls when an element’s value changes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
typealias GCMicroGamepadValueChangedHandler = (GCMicroGamepad, GCControllerElement) -> Void
```

## Parameters 

`gamepad`  

The profile whose element value changes.

`element`  

The element in the profile whose value changes.

## See Also

### Receiving a callback when input values change

var valueChangedHandler: GCMicroGamepadValueChangedHandler?

The block that this profile calls when an element’s value changes.

