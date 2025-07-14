

- Game Controller
-  GCMouseInput 

Class

# GCMouseInput

A controller profile that tracks input from a mouse.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class GCMouseInput
```

## Overview

This profile supports a mouse with the following features:

- A two-axis cursor and scroll

- A left button

- An optional right button

- An optional middle button

- An optional set of auxiliarly buttons

This profile provides only raw mouse movement delta values. For the cursor position at a specific time, use the UIHoverGestureRecognizer class and the `NSEvent` mouseLocation method.

## Topics

### Getting Change Information

var mouseMovedHandler: GCMouseMoved?

The block that the profile calls when the mouse moves.

typealias GCMouseMoved

The signature for the block that the mouse input profile calls when the mouse moves.

### Accessing Buttons

var leftButton: GCControllerButtonInput

The left button on the mouse.

var rightButton: GCControllerButtonInput?

The optional right button on the mouse.

var middleButton: GCControllerButtonInput?

The optional middle button on the mouse.

var auxiliaryButtons: [GCControllerButtonInput]?

The optional additional buttons on the mouse.

### Scrolling

var scroll: GCDeviceCursor

The location of the directional pad cursor with an undefined range.

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

class GCKeyboardInput

A controller profile that uses the keyboard as the input device.

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

