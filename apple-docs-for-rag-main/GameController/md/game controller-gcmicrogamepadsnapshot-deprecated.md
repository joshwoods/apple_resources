

- Game Controller
-  GCMicroGamepadSnapshot Deprecated

Class

# GCMicroGamepadSnapshot

A recording of all of the values provided by a GCMicroGamepad object.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class GCMicroGamepadSnapshot
```

Deprecated

Use the withMicroGamepad() method instead.

## Overview

To create a gamepad snapshot, call the saveSnapshot() method on a GCMicroGamepad object. The GCMicroGamepadSnapshot class is a subclass of the GCMicroGamepad class, so you use the parent class’s properties to read the individual element values. The snapshot is stored in a device independent format. To get the flattened data representation of the snapshot data, read the snapshotData property.

## Topics

### Converting Between Snapshots and Data Objects

init(snapshotData: Data)

Initializes a snapshot object with the flattened data representation obtained from another snapshot.

init(controller: GCController, snapshotData: Data)

var snapshotData: Data

The flattened control input values for the snapshot.

### Flattening a Snapshot to Memory

struct GCMicroGamepadSnapShotDataV100

A structure that holds a snapshot of a micro gamepad controller’s input data.

func NSDataFromGCMicroGamepadSnapShotDataV100(UnsafeMutablePointer&lt;GCMicroGamepadSnapShotDataV100>?) -> Data?

Encapsulates the controller data from a micro gamepad structure into a data object.

func GCMicroGamepadSnapShotDataV100FromNSData(UnsafeMutablePointer&lt;GCMicroGamepadSnapShotDataV100>?, Data?) -> Bool

Copies the recorded data from a micro gamepad snapshot into a readable structure.

## Relationships

### Inherits From

- GCMicroGamepad

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

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

struct GCExtendedGamepadSnapshotDataDeprecated

struct GCMicroGamepadSnapshotDataDeprecated

enum GCExtendedGamepadSnapshotDataVersionDeprecated

enum GCMicroGamepadSnapshotDataVersionDeprecated

let GCCurrentExtendedGamepadSnapshotDataVersion: GCExtendedGamepadSnapshotDataVersionDeprecated

let GCCurrentMicroGamepadSnapshotDataVersion: GCMicroGamepadSnapshotDataVersionDeprecated

func GCExtendedGamepadSnapshotDataFromNSData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapshotData>?, Data?) -> BoolDeprecated

func GCMicroGamepadSnapshotDataFromNSData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?, Data?) -> BoolDeprecated

func NSDataFromGCExtendedGamepadSnapshotData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapshotData>?) -> Data?Deprecated

func NSDataFromGCMicroGamepadSnapshotData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?) -> Data?Deprecated

