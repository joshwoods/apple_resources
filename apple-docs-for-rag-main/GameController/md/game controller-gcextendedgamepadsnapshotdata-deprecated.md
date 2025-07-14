

- Game Controller
-  GCExtendedGamepadSnapshotData Deprecated

Structure

# GCExtendedGamepadSnapshotData

iOS 13.0–13.0DeprecatediPadOS 13.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.15–10.15DeprecatedtvOS 13.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
struct GCExtendedGamepadSnapshotData
```

Deprecated

Use the -\[GCController controllerWithExtendedGamepad\] method instead

## Topics

### Initializers

init()

init(version: UInt16, size: UInt16, dpadX: Float, dpadY: Float, buttonA: Float, buttonB: Float, buttonX: Float, buttonY: Float, leftShoulder: Float, rightShoulder: Float, leftThumbstickX: Float, leftThumbstickY: Float, rightThumbstickX: Float, rightThumbstickY: Float, leftTrigger: Float, rightTrigger: Float, supportsClickableThumbsticks: ObjCBool, leftThumbstickButton: ObjCBool, rightThumbstickButton: ObjCBool)

### Instance Properties

var buttonA: Float

var buttonB: Float

var buttonX: Float

var buttonY: Float

var dpadX: Float

var dpadY: Float

var leftShoulder: Float

var leftThumbstickButton: ObjCBool

var leftThumbstickX: Float

var leftThumbstickY: Float

var leftTrigger: Float

var rightShoulder: Float

var rightThumbstickButton: ObjCBool

var rightThumbstickX: Float

var rightThumbstickY: Float

var rightTrigger: Float

var size: UInt16

var supportsClickableThumbsticks: ObjCBool

var version: UInt16

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Deprecated symbols

class GCGamepad

The standard set of gamepad controls.

Deprecated

class GCExtendedGamepadSnapshot

A recording of all of the values provided by a GCExtendedGamepad object.

Deprecated

class GCGamepadSnapshot

A recording of all of the values provided by a GCGamepad object.

Deprecated

class GCMicroGamepadSnapshot

A recording of all of the values provided by a GCMicroGamepad object.

Deprecated

struct GCMicroGamepadSnapshotDataDeprecated

enum GCExtendedGamepadSnapshotDataVersionDeprecated

enum GCMicroGamepadSnapshotDataVersionDeprecated

let GCCurrentExtendedGamepadSnapshotDataVersion: GCExtendedGamepadSnapshotDataVersionDeprecated

let GCCurrentMicroGamepadSnapshotDataVersion: GCMicroGamepadSnapshotDataVersionDeprecated

func GCExtendedGamepadSnapshotDataFromNSData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapshotData>?, Data?) -> BoolDeprecated

func GCMicroGamepadSnapshotDataFromNSData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?, Data?) -> BoolDeprecated

func NSDataFromGCExtendedGamepadSnapshotData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapshotData>?) -> Data?Deprecated

func NSDataFromGCMicroGamepadSnapshotData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?) -> Data?Deprecated

