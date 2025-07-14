

- Game Controller
-  GCExtendedGamepadSnapshot Deprecated

Class

# GCExtendedGamepadSnapshot

A recording of all of the values provided by a GCExtendedGamepad object.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class GCExtendedGamepadSnapshot
```

Deprecated

Use the withExtendedGamepad() method instead.

## Overview

To create a gamepad snapshot, call the saveSnapshot() method on a GCExtendedGamepad object. The GCExtendedGamepadSnapshot class is a subclass of the GCExtendedGamepad class, so you use the parent class’s properties to read the individual element values. The snapshot is stored in a device independent format. To get the flattened data representation of the snapshot data, read the snapshotData property.

## Topics

### Converting Between Extended Snapshots and Data Objects

init(snapshotData: Data)

Initializes a snapshot object with the flattened data representation obtained from another snapshot.

init(controller: GCController, snapshotData: Data)

Initializes a snapshot object associated with a specific controller using a flattened data representation obtained from another snapshot.

var snapshotData: Data

Flattens a snapshot into an archivable memory representation.

### Flattening a Snapshot to Memory

struct GCExtendedGamepadSnapShotDataV100

A structure that holds a snapshot of an extended gamepad controller’s input data.

func NSDataFromGCExtendedGamepadSnapShotDataV100(UnsafeMutablePointer&lt;GCExtendedGamepadSnapShotDataV100>?) -> Data?

Encapsulates the controller data from an extended gamepad structure into a data object.

func GCExtendedGamepadSnapShotDataV100FromNSData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapShotDataV100>?, Data?) -> Bool

Copies the recorded data from an extended gamepad snapshot into a readable structure.

## Relationships

### Inherits From

- GCExtendedGamepad

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

func GCExtendedGamepadSnapshotDataFromNSData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapshotData>?, Data?) -> BoolDeprecated

func GCMicroGamepadSnapshotDataFromNSData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?, Data?) -> BoolDeprecated

func NSDataFromGCExtendedGamepadSnapshotData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapshotData>?) -> Data?Deprecated

func NSDataFromGCMicroGamepadSnapshotData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?) -> Data?Deprecated

