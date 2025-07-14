

- Game Controller
-  GCCurrentMicroGamepadSnapshotDataVersion Deprecated

Global Variable

# GCCurrentMicroGamepadSnapshotDataVersion

iOS 13.0–13.0DeprecatediPadOS 13.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.15–10.15DeprecatedtvOS 13.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
let GCCurrentMicroGamepadSnapshotDataVersion: GCMicroGamepadSnapshotDataVersion
```

Deprecated

Use the withMicroGamepad() method instead.

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

struct GCExtendedGamepadSnapshotDataDeprecated

struct GCMicroGamepadSnapshotDataDeprecated

enum GCExtendedGamepadSnapshotDataVersionDeprecated

enum GCMicroGamepadSnapshotDataVersionDeprecated

let GCCurrentExtendedGamepadSnapshotDataVersion: GCExtendedGamepadSnapshotDataVersionDeprecated

func GCExtendedGamepadSnapshotDataFromNSData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapshotData>?, Data?) -> BoolDeprecated

func GCMicroGamepadSnapshotDataFromNSData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?, Data?) -> BoolDeprecated

func NSDataFromGCExtendedGamepadSnapshotData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapshotData>?) -> Data?Deprecated

func NSDataFromGCMicroGamepadSnapshotData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?) -> Data?Deprecated

