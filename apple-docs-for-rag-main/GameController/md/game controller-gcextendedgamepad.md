

- Game Controller
-  GCExtendedGamepad 

Class

# GCExtendedGamepad

A controller profile that supports the extended set of gamepad controls.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class GCExtendedGamepad
```

## Overview

The extended gamepad controller profile represents a physical or virtual controller with the following input elements:

- Two shoulder buttons

- Two trigger buttons

- Four face buttons in a diamond pattern

- One directional pad

- Two thumbsticks with optional thumbstick buttons

- Optional Home and Options buttons

- A Menu button

If a GCController object supports this type of profile, get the input values of the elements from the controller’s extendedGamepad property or use the profile’s valueChangedHandler method to receive a callback when the input values change. Alternatively, use the saveSnapshot() method to capture the input values at a moment in time.

If the controller’s extendedGamepad property is `nil`, the controller doesn’t support this type of profile. See GCController for other profiles you can use.

## Topics

### Getting the controller

var controller: GCController?

The controller for the profile.

### Getting change information

var valueChangedHandler: GCExtendedGamepadValueChangedHandler?

The block that the profile calls when an element’s value changes.

typealias GCExtendedGamepadValueChangedHandler

The signature for the block that the profile calls when an element’s value changes.

### Getting shoulder button inputs

var leftShoulder: GCControllerButtonInput

The controller’s left shoulder button element.

var rightShoulder: GCControllerButtonInput

The controller’s right shoulder button element.

### Getting trigger inputs

var leftTrigger: GCControllerButtonInput

The controller’s left trigger element.

var rightTrigger: GCControllerButtonInput

The controller’s right trigger element.

### Getting face button inputs

var buttonMenu: GCControllerButtonInput

The primary menu button element that players use to enter the main menu and pause the game.

var buttonOptions: GCControllerButtonInput?

The controller’s secondary menu button element.

var buttonHome: GCControllerButtonInput?

The main menu button element that players use to enter the secondary menu and pause the game.

var buttonA: GCControllerButtonInput

The bottom face button that uses *A* or another indicator as its label.

var buttonB: GCControllerButtonInput

The right face button that uses *B* or another indicator as its label.

var buttonX: GCControllerButtonInput

The left face button that uses *X* or another indicator as its label.

var buttonY: GCControllerButtonInput

The top face button that uses *Y* or another indicator as its label.

### Getting directional pad inputs

var dpad: GCControllerDirectionPad

The controller’s directional pad element.

### Getting thumbstick and thumbstick button inputs

var leftThumbstick: GCControllerDirectionPad

The controller’s left thumbstick element.

var rightThumbstick: GCControllerDirectionPad

The controller’s right thumbstick element.

var leftThumbstickButton: GCControllerButtonInput?

The button on the left thumbstick of the controller.

var rightThumbstickButton: GCControllerButtonInput?

The button on the right thumbstick of the controller.

### Accessing elements by name

Extended gamepad input names

Constants for names of extended gamepad elements.

### Setting snapshot values

func setStateFrom(GCExtendedGamepad)

Copies the input values from a specified extended gamepad to a snapshot of an extended gamepad.

func saveSnapshot() -> GCExtendedGamepadSnapshot

Saves a snapshot of all of the profile’s elements.

Deprecated

## Relationships

### Inherits From

- GCPhysicalInputProfile

### Inherited By

- GCDualSenseGamepad
- GCDualShockGamepad
- GCExtendedGamepadSnapshot
- GCXboxGamepad

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

