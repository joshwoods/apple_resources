

- Game Controller
-  GCMicroGamepadSnapShotDataV100 Deprecated

Structure

# GCMicroGamepadSnapShotDataV100

A structure that holds a snapshot of a micro gamepad controller’s input data.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
struct GCMicroGamepadSnapShotDataV100
```

Deprecated

Use the -\[GCController controllerWithMicroGamepad\] method instead

## Topics

### Instance Properties

var buttonA: Float

The value of the A button.

var buttonX: Float

var dpadX: Float

The value of the horizontal axis of the dpad.

var dpadY: Float

The value of the vertical axis of the dpad.

var size: UInt16

The size of the recorded structure, in bytes.

var version: UInt16

A value that indicates the version number of the data structure.

### Initializers

init()

init(version: UInt16, size: UInt16, dpadX: Float, dpadY: Float, buttonA: Float, buttonX: Float)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Flattening a Snapshot to Memory

func NSDataFromGCMicroGamepadSnapShotDataV100(UnsafeMutablePointer&lt;GCMicroGamepadSnapShotDataV100>?) -> Data?

Encapsulates the controller data from a micro gamepad structure into a data object.

Deprecated

func GCMicroGamepadSnapShotDataV100FromNSData(UnsafeMutablePointer&lt;GCMicroGamepadSnapShotDataV100>?, Data?) -> Bool

Copies the recorded data from a micro gamepad snapshot into a readable structure.

Deprecated

