

- Game Controller
-  Input 

API Collection

# Input

Receive controller input in the way that best integrates with the flow of your game or game engine.

## Topics

### Essentials

Handling input events

Receive controller input using either polling or callbacks.

protocol GCDevicePhysicalInput

The common properties and methods for objects that represent the input profile of a device.

protocol GCDevicePhysicalInputState

The common properties for physical devices with elements.

protocol GCDevicePhysicalInputStateDiff

The common functions for objects that contain the differences between a current and previous input state object.

### Elements

struct GCPhysicalInputElementCollection

A collection of physical input elements.

protocol GCPhysicalInputElement

The common properties of physical input elements.

protocol GCButtonElement

The common properties of an element that represents a momentary switch, such as a push button.

protocol GCAxisElement

The common properties for an element that represents an absolute or relative input value along an axis.

protocol GCSwitchElement

The common properties for an element that represents a switch.

protocol GCDirectionPadElement

The common properties of elements that represent directional pads.

### Element inputs

protocol GCPhysicalInputSource

A protocol for a description of an element without any system-level remapping of the controls.

### Element names

struct GCPhysicalInputElementName

The name of a physical input element.

protocol GCPhysicalInputElementTypedName

A type-safe name for accessing elements of a physical input element collection.

struct GCButtonElementName

The names of the button elements.

struct GCAxisElementName

The names for the elements that provide values along an axis.

struct GCSwitchElementName

The name for an element that represents a switch.

struct GCDirectionPadElementName

The names for directional pad elements.

Extended gamepad input names

Constants for names of extended gamepad elements.

DualShock controller input names

Constants for names of DualShock 4 elements.

Xbox controller input names

Constants for names of Xbox elements.

Micro gamepad input names

Constants for names of micro gamepad elements.

Directional Gamepad Input Names

Constants for names of directional pad elements.

## See Also

### Game controller profiles

class GCMotion

A controller profile that supports orientation and motion.

class GCDeviceBattery

The charge level and state of a device’s battery.

class GCDeviceHaptics

The locations of haptic actuators on a game controller.

class GCDeviceLight

The colored light on a device.

