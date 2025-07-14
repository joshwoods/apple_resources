

- Game Controller
-  GCExtendedGamepadSnapShotDataV100 Deprecated

Structure

# GCExtendedGamepadSnapShotDataV100

A structure that holds a snapshot of an extended gamepad controller’s input data.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
struct GCExtendedGamepadSnapShotDataV100
```

Deprecated

Use the -\[GCController controllerWithExtendedGamepad\] method instead

## Topics

### Instance Properties

var buttonA: Float

The value of the A button.

var buttonB: Float

The value of the B button.

var buttonX: Float

The value of the X button.

var buttonY: Float

The value of the Y button.

var dpadX: Float

The value of the horizontal axis of the dpad.

var dpadY: Float

The value of the vertical axis of the dpad.

var leftShoulder: Float

The value of the left shoulder button.

var leftThumbstickX: Float

The value of the horizontal axis of the left thumbstick.

var leftThumbstickY: Float

The value of the vertical axis of the left thumbstick.

var leftTrigger: Float

The value of the left trigger.

var rightShoulder: Float

The value of the right shoulder button.

var rightThumbstickX: Float

The value of the horizontal axis of the right thumbstick.

var rightThumbstickY: Float

The value of the vertical axis of the right thumbstick.

var rightTrigger: Float

The value of the right trigger.

var size: UInt16

The size of the recorded structure, in bytes.

var version: UInt16

A value that indicates the version number of the data structure.

### Initializers

init()

init(version: UInt16, size: UInt16, dpadX: Float, dpadY: Float, buttonA: Float, buttonB: Float, buttonX: Float, buttonY: Float, leftShoulder: Float, rightShoulder: Float, leftThumbstickX: Float, leftThumbstickY: Float, rightThumbstickX: Float, rightThumbstickY: Float, leftTrigger: Float, rightTrigger: Float)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Flattening a Snapshot to Memory

func NSDataFromGCExtendedGamepadSnapShotDataV100(UnsafeMutablePointer&lt;GCExtendedGamepadSnapShotDataV100>?) -> Data?

Encapsulates the controller data from an extended gamepad structure into a data object.

Deprecated

func GCExtendedGamepadSnapShotDataV100FromNSData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapShotDataV100>?, Data?) -> Bool

Copies the recorded data from an extended gamepad snapshot into a readable structure.

Deprecated

