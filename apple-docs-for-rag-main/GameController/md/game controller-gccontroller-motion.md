

- Game Controller
- GCController
-  motion 

Instance Property

# motion

The motion input profile.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var motion: GCMotion? { get }
```

## Discussion

If the controller supports the motion profile, this property is a GCMotion object that you use to access the controller’s motion data. If the controller doesn’t support the motion input profile, this property is `nil`.

## See Also

### Accessing controller profiles

var extendedGamepad: GCExtendedGamepad?

The extended gamepad profile.

class GCPhysicalInputProfile

The base class for controller profiles that support physical buttons, thumbsticks, and directional pads.

class GCKeyboardInput

A controller profile that uses the keyboard as the input device.

class GCMouseInput

A controller profile that tracks input from a mouse.

class GCExtendedGamepad

A controller profile that supports the extended set of gamepad controls.

class GCDualShockGamepad

A controller profile that supports the DualShock 4 controller.

class GCXboxGamepad

A controller profile that supports the Xbox controller.

class GCDualSenseGamepad

A controller profile that supported the DualSense controller.

var microGamepad: GCMicroGamepad?

The micro gamepad profile.

class GCMicroGamepad

A controller profile that supports the Siri Remote.

class GCDirectionalGamepad

A profile that supports only the directional pad, without motion or rotation.

var physicalInputProfile: GCPhysicalInputProfile

The physical input profile for the controller.

var gamepad: GCGamepad?

The gamepad profile.

Deprecated

