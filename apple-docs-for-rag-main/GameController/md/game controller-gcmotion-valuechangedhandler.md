

- Game Controller
- GCMotion
-  valueChangedHandler 

Instance Property

# valueChangedHandler

The block that the profile calls when an element’s value changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var valueChangedHandler: GCMotionValueChangedHandler? { get set }
```

## Discussion

If multiple elements change values at the same time, the profile calls this block once for each element that changes. If the value of a subelement changes, the profile only calls the block for the containing element.

## See Also

### Receiving a Callback When Input Values Change

typealias GCMotionValueChangedHandler

The signature for the block that the profile calls when an element’s value changes.

