

- Game Controller
-  GCExtendedGamepadSnapshotDataFromNSData(\_:\_:) Deprecated

Function

# GCExtendedGamepadSnapshotDataFromNSData(\_:\_:)

iOS 13.0–13.0DeprecatediPadOS 13.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.15–10.15DeprecatedtvOS 13.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func GCExtendedGamepadSnapshotDataFromNSData(
    _ snapshotData: UnsafeMutablePointer?,
    _ data: Data?
) -> Bool
```

Deprecated

Use the withExtendedGamepad() method instead.

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

let GCCurrentMicroGamepadSnapshotDataVersion: GCMicroGamepadSnapshotDataVersionDeprecated

func GCMicroGamepadSnapshotDataFromNSData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?, Data?) -> BoolDeprecated

func NSDataFromGCExtendedGamepadSnapshotData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapshotData>?) -> Data?Deprecated

func NSDataFromGCMicroGamepadSnapshotData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?) -> Data?Deprecated

