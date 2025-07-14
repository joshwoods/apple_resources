

- Game Controller
-  GCGamepadSnapShotDataV100 Deprecated

Structure

# GCGamepadSnapShotDataV100

A structure that holds a snapshot of a gamepad controller’s input data.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
struct GCGamepadSnapShotDataV100
```

Deprecated

Use GCExtendedGamepad instead

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

var rightShoulder: Float

The value of the right shoulder button.

var size: UInt16

The size of the recorded structure, in bytes.

var version: UInt16

A value that indicates the version number of the data structure.

### Initializers

init()

init(version: UInt16, size: UInt16, dpadX: Float, dpadY: Float, buttonA: Float, buttonB: Float, buttonX: Float, buttonY: Float, leftShoulder: Float, rightShoulder: Float)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Flattening a Snapshot to Memory

func NSDataFromGCGamepadSnapShotDataV100(UnsafeMutablePointer&lt;GCGamepadSnapShotDataV100>?) -> Data?

Encapsulates the controller data from a gamepad structure into a data object.

Deprecated

func GCGamepadSnapShotDataV100FromNSData(UnsafeMutablePointer&lt;GCGamepadSnapShotDataV100>?, Data?) -> Bool

Copies the recorded data from a gamepad snapshot into a readable structure.

Deprecated

