

- Game Controller
-  GCMicroGamepad 

Class

# GCMicroGamepad

A controller profile that supports the Siri Remote.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GCMicroGamepad
```

## Overview

The micro gamepad controller profile supports the following input elements:

- Two digital face buttons (A and X).

- One analog directional pad (D-pad) that functions as a touchpad.

Users can rotate game controllers that support the micro gamepad profile, switching them between landscape and portrait orientation. If you want to get directional values according to the orientation, set the allowsRotation property to true.

## Topics

### Getting the controller

var controller: GCController?

The controller associated with this profile.

### Receiving a callback when input values change

var valueChangedHandler: GCMicroGamepadValueChangedHandler?

The block that this profile calls when an element’s value changes.

typealias GCMicroGamepadValueChangedHandler

Signature for the block that this profile calls when an element’s value changes.

### Getting face button inputs

var buttonMenu: GCControllerButtonInput

The menu face button that players use to enter the main menu and pause the game.

var buttonA: GCControllerButtonInput

The button that the user activates by pressing harder on the touchpad.

var buttonX: GCControllerButtonInput

The second face button element.

### Getting directional pad inputs

var dpad: GCControllerDirectionPad

The controller’s directional pad element.

var reportsAbsoluteDpadValues: Bool

A Boolean value that indicates whether the directional pad reports absolute or relative values.

var allowsRotation: Bool

A Boolean value that indicates whether the profile reports the directional pad values relative to its current orientation.

### Accessing elements by name

Micro gamepad input names

Constants for names of micro gamepad elements.

### Setting snapshot avlues

func setStateFrom(GCMicroGamepad)

Copies the input values from a specified micro gamepad to a snapshot of a micro gamepad.

func saveSnapshot() -> GCMicroGamepadSnapshot

Saves a snapshot of all of the profile’s elements.

Deprecated

## Relationships

### Inherits From

- GCPhysicalInputProfile

### Inherited By

- GCDirectionalGamepad
- GCMicroGamepadSnapshot

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

class GCDirectionalGamepad

A profile that supports only the directional pad, without motion or rotation.

var motion: GCMotion?

The motion input profile.

var physicalInputProfile: GCPhysicalInputProfile

The physical input profile for the controller.

var gamepad: GCGamepad?

The gamepad profile.

Deprecated

