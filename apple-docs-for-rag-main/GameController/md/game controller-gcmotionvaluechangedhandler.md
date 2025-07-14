

- Game Controller
-  GCMotionValueChangedHandler 

Type Alias

# GCMotionValueChangedHandler

The signature for the block that the profile calls when an element’s value changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
typealias GCMotionValueChangedHandler = (GCMotion) -> Void
```

## Parameters 

`motion`  

The profile with the element values that change.

## See Also

### Receiving a Callback When Input Values Change

var valueChangedHandler: GCMotionValueChangedHandler?

The block that the profile calls when an element’s value changes.

