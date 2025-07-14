

- Game Controller
-  GCButtonElementName 

Structure

# GCButtonElementName

The names of the button elements.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS

``` source
struct GCButtonElementName
```

## Topics

### Getting extended gamepad shoulder button names

static let leftShoulder: GCButtonElementName

The name of the left shoulder button.

static let rightShoulder: GCButtonElementName

The name of the right shoulder button.

static let leftBumper: GCButtonElementName

The name of the additional left shoulder button.

static let rightBumper: GCButtonElementName

The name of the additional right shoulder button.

### Getting extended gamepad trigger names

static let leftTrigger: GCButtonElementName

The name of the left trigger.

static let rightTrigger: GCButtonElementName

The name of the right trigger.

### Getting extended gamepad face button names

static let menu: GCButtonElementName

The name of the primary menu button element.

static let options: GCButtonElementName

The name of the main options button element.

static let home: GCButtonElementName

The name of the main menu button element.

static let a: GCButtonElementName

The name for the controller’s A button.

static let b: GCButtonElementName

The name for the controller’s B button.

static let x: GCButtonElementName

The name for the controller’s X button.

static let y: GCButtonElementName

The name for the controller’s Y button.

### Getting extended gamepad thumbstick names

static let leftThumbstickButton: GCButtonElementName

The name of the left thumbstick element.

static let rightThumbstickButton: GCButtonElementName

The name of the right thumbstick element.

### Getting extended gamepad back button names

Some gamepads include additional buttons or triggers on their underside. Because the number and layout of bottom buttons vary by controller, the Game Controller framework identifies them by their easy of use or position to the person’s fingers.

static func backLeftButton(position: Int) -> GCButtonElementName

Returns the name of the back left button at the specified location.

static func backRightButton(position: Int) -> GCButtonElementName

Returns the name of the back right button at the specified location.

### Getting steering wheel controller names

static let pedalClutch: GCButtonElementName

The name of the controller’s clutch.

static let pedalBrake: GCButtonElementName

The name of the controller’s brake pedal.

static let pedalAccelerator: GCButtonElementName

The name of the controller’s accelerator pedal.

static let leftPaddle: GCButtonElementName

The name of the controller’s left paddle.

static let rightPaddle: GCButtonElementName

The name of the controller’s right paddle.

### Getting Xbox button names

static let share: GCButtonElementName

The name of the Xbox share button.

### Getting arcade stick button names

static func arcadeButton(row: Int, column: Int) -> GCButtonElementName

Returns the name of the arcade stick button at the specified location.

## Relationships

### Conforms To

- Copyable
- Equatable
- GCPhysicalInputElementTypedName
- Hashable
- RawRepresentable
- Sendable

## See Also

### Element names

struct GCPhysicalInputElementName

The name of a physical input element.

protocol GCPhysicalInputElementTypedName

A type-safe name for accessing elements of a physical input element collection.

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

