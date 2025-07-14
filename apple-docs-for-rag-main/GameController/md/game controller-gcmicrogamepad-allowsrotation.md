

- Game Controller
- GCMicroGamepad
-  allowsRotation 

Instance Property

# allowsRotation

A Boolean value that indicates whether the profile reports the directional pad values relative to its current orientation.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var allowsRotation: Bool { get set }
```

## Discussion

If this property is false, the profile reports the value of the directional pad only in portrait orientation even when the user rotates the controller. If this property is true, the profile reports the values using the current orientation. The default value for this property is false.

## See Also

### Getting directional pad inputs

var dpad: GCControllerDirectionPad

The controller’s directional pad element.

var reportsAbsoluteDpadValues: Bool

A Boolean value that indicates whether the directional pad reports absolute or relative values.

