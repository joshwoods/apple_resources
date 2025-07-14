

- Game Controller
- GCMicroGamepad
-  reportsAbsoluteDpadValues 

Instance Property

# reportsAbsoluteDpadValues

A Boolean value that indicates whether the directional pad reports absolute or relative values.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var reportsAbsoluteDpadValues: Bool { get set }
```

## Discussion

If this property is false, the profile assumes the location where the user first touches the pad is the origin value (`0.0,0.0`) for the pad. The profile calculates all subsequent values relative to this position until the user lifts their finger. The next time the user touches the pad, the profile uses that location as the new origin. If this property is true, the profile calculates values relative to the physical center of the touchpad. The default value for this property is false.

## See Also

### Getting directional pad inputs

var dpad: GCControllerDirectionPad

The controller’s directional pad element.

var allowsRotation: Bool

A Boolean value that indicates whether the profile reports the directional pad values relative to its current orientation.

