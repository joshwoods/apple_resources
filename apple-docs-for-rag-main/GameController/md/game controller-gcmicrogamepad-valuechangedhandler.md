

- Game Controller
- GCMicroGamepad
-  valueChangedHandler 

Instance Property

# valueChangedHandler

The block that this profile calls when an element’s value changes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var valueChangedHandler: GCMicroGamepadValueChangedHandler? { get set }
```

## Discussion

If multiple elements change values at the same time, the profile calls this block once for each element that changed. If the value of a child element changes, the profile only calls the block for the containing element.

## See Also

### Receiving a callback when input values change

typealias GCMicroGamepadValueChangedHandler

Signature for the block that this profile calls when an element’s value changes.

