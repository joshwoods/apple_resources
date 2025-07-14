

- Game Controller
-  GCKeyboardInput 

Class

# GCKeyboardInput

A controller profile that uses the keyboard as the input device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class GCKeyboardInput
```

## Overview

Use this profile to get the state of the keyboard buttons that the GCKeyCode structure defines.

## Topics

### Getting Change Information

var keyChangedHandler: GCKeyboardValueChangedHandler?

The block that the profile calls when the user presses a key.

typealias GCKeyboardValueChangedHandler

The signature for the block that the keyboard input profile calls when a key value changes.

### Accessing Buttons

var isAnyKeyPressed: Bool

A Boolean value that indicates whether the user is pressing any of the keys.

func button(forKeyCode: GCKeyCode) -> GCControllerButtonInput?

Returns the button element for the specified key code.

struct GCKeyCode

The key codes for keys on a keyboard.

Keycode Constants

Constants for the codes of keyboard keys.

## Relationships

### Inherits From

- GCPhysicalInputProfile

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

var motion: GCMotion?

The motion input profile.

var physicalInputProfile: GCPhysicalInputProfile

The physical input profile for the controller.

var gamepad: GCGamepad?

The gamepad profile.

Deprecated

