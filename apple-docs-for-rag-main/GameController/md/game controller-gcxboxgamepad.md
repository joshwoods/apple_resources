

- Game Controller
-  GCXboxGamepad 

Class

# GCXboxGamepad

A controller profile that supports the Xbox controller.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class GCXboxGamepad
```

## Overview

The Xbox controller profile is similar to an extended game pad (GCExtendedGamepad), but has four paddle button elements.

## Topics

### Getting button inputs

var paddleButton1: GCControllerButtonInput?

The controller’s paddle 1 button element, which has a P1 label on the back of the controller.

var paddleButton2: GCControllerButtonInput?

The paddle 2 button element, which has a P2 label on the back of the controller.

var paddleButton3: GCControllerButtonInput?

The paddle 3 button element, which has a P3 label on the back of the controller.

var paddleButton4: GCControllerButtonInput?

The paddle 4 button element, which has a P4 label on the back of the controller.

var buttonShare: GCControllerButtonInput?

The share button on an Xbox Series X\|S controller or later.

### Accessing elements by name

Xbox controller input names

Constants for names of Xbox elements.

## Relationships

### Inherits From

- GCExtendedGamepad

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

class GCDualSenseGamepad

A controller profile that supported the DualSense controller.

var microGamepad: GCMicroGamepad?

The micro gamepad profile.

class GCMicroGamepad

A controller profile that supports the Siri Remote.

class GCDirectionalGamepad

A profile that supports only the directional pad, without motion or rotation.

var motion: GCMotion?

The motion input profile.

var physicalInputProfile: GCPhysicalInputProfile

The physical input profile for the controller.

var gamepad: GCGamepad?

The gamepad profile.

Deprecated

