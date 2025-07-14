

- Game Controller
-  GCPhysicalInputProfile 

Class

# GCPhysicalInputProfile

The base class for controller profiles that support physical buttons, thumbsticks, and directional pads.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class GCPhysicalInputProfile
```

## Overview

This class provides properties and methods for accessing common elements of controllers, and for creating snapshots of profiles.

## Topics

### Getting the device

var device: (any GCDevice)?

The physical device that the profile represents.

### Getting change information

var lastEventTimestamp: TimeInterval

The time of the most recent change to an element’s value.

var valueDidChangeHandler: ((GCPhysicalInputProfile, GCControllerElement) -> Void)?

The block that the profile calls when an element’s value changes.

### Accessing elements by name or key

var elements: [String : GCControllerElement]

The elements in the profile as key-value pairs for lookup by name.

var buttons: [String : GCControllerButtonInput]

The buttons in the profile as key-value pairs for lookup by name.

var axes: [String : GCControllerAxisInput]

The axes in the profile as key-value pairs for lookup by name.

var dpads: [String : GCControllerDirectionPad]

The directional pads in the profile as key-value pairs for lookup by name.

var touchpads: [String : GCControllerTouchpad]

The touchpads in the profile as key-value pairs for lookup by name.

subscript(String) -> GCControllerElement?

Returns the element that the key specifies.

### Getting elements by type

var allElements: Set&lt;GCControllerElement>

The elements in the profile.

var allButtons: Set&lt;GCControllerButtonInput>

The buttons in the profile.

var allAxes: Set&lt;GCControllerAxisInput>

The axes in the profile.

var allDpads: Set&lt;GCControllerDirectionPad>

The directional pads in the profile.

var allTouchpads: Set&lt;GCControllerTouchpad>

The touchpads in the profile.

### Setting snapshot values

func capture() -> Self

Returns a snapshot of the profile with its current element values.

func setStateFromPhysicalInput(GCPhysicalInputProfile)

Copies the input values from a specified physical input profile to a snapshot of the profile.

### Remapping input elements

var hasRemappedElements: Bool

A Boolean value that indicates whether the user remaps elements in this profile.

func mappedElementAlias(forPhysicalInputName: String) -> String

Returns the name of the input element to which the user remaps the given physical element.

func mappedPhysicalInputNames(forElementAlias: String) -> Set&lt;String>

Returns the physical input elements to which the user remaps the given input element.

static let GCControllerUserCustomizationsDidChange: NSNotification.Name

A notification that posts when the user customizes the button mappings or other settings of a controller.

## Relationships

### Inherits From

- NSObject

### Inherited By

- GCExtendedGamepad
- GCGamepad
- GCKeyboardInput
- GCMicroGamepad
- GCMouseInput

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

var motion: GCMotion?

The motion input profile.

var physicalInputProfile: GCPhysicalInputProfile

The physical input profile for the controller.

var gamepad: GCGamepad?

The gamepad profile.

Deprecated

