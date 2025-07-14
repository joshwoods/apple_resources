

- Game Controller
-  GCDirectionalGamepad 

Class

# GCDirectionalGamepad

A profile that supports only the directional pad, without motion or rotation.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+macOS 11.1+tvOS 14.3+visionOS 1.0+

``` source
class GCDirectionalGamepad
```

## Overview

The directional gamepad profile is similar to a micro gamepad profile except it doesn’t support motion or rotation. The controller’s motion property is `nil` and the inherited allowsRotation property is false.

If you select Micro Gamepad when you add the Game Controllers capability (GCSupportedGameControllers ) to your project, and you also support the GCDirectionalGamepad profile, select Directional Gamepad as well.

If you support the second-generation Siri Remote and later, set the GCSupportsMultipleMicroGamepads key to `YES` in the information property list in your project.

In addition, the directional pad element may report digital or analog values. If the directional pad’s isAnalog property is false, it reports absolute directional pad values (the reportsAbsoluteDpadValues property is true).

## Topics

### Accessing Elements by Name

Directional Gamepad Input Names

Constants for names of directional pad elements.

## Relationships

### Inherits From

- GCMicroGamepad

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

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

var motion: GCMotion?

The motion input profile.

var physicalInputProfile: GCPhysicalInputProfile

The physical input profile for the controller.

var gamepad: GCGamepad?

The gamepad profile.

Deprecated

