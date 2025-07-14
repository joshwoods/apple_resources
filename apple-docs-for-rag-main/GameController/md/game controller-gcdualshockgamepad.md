

- Game Controller
-  GCDualShockGamepad 

Class

# GCDualShockGamepad

A controller profile that supports the DualShock 4 controller.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class GCDualShockGamepad
```

## Overview

The DualShock 4 controller profile is similar to an extended gamepad (GCExtendedGamepad), but has a touchpad with a button and two-finger tracking.

This profile also supports motion — that is, the controller’s motion property is non-nil. If you hold the controller in front of you, the direction of the axes are:

- The positive x-axis points to your right.

- The positive y-axis points up.

- The positive z-axis starts at the touchpad and points to you.

## Topics

### Getting button input

var touchpadButton: GCControllerButtonInput!

The button element on the touchpad of the controller.

### Tracking finger locations

var touchpadPrimary: GCControllerDirectionPad!

The location of the player’s primary finger on the touchpad.

var touchpadSecondary: GCControllerDirectionPad!

The location of the player’s secondary finger on the touchpad.

### Accessing elements by name

DualShock controller input names

Constants for names of DualShock 4 elements.

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

