

- Game Controller
-  GCGamepad Deprecated

Class

# GCGamepad

The standard set of gamepad controls.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class GCGamepad
```

## Overview

The controls associated with the gamepad profile include the following:

- Two shoulder buttons.

- Four face buttons arranged in a diamond pattern.

- One directional pad (D-pad).

## Topics

### Determining the Controller That Owns This Profile

var controller: GCController?

The controller this profile is associated with.

### Determining When Any Element in the Profile Changes

var valueChangedHandler: GCGamepadValueChangedHandler?

A block called when any element in the profile changes.

### Reading Shoulder Button Inputs

var leftShoulder: GCControllerButtonInput

The left shoulder button element.

var rightShoulder: GCControllerButtonInput

The right shoulder button element.

### Reading Directional Pad Inputs

var dpad: GCControllerDirectionPad

The D-pad element.

### Reading Face Button Inputs

var buttonA: GCControllerButtonInput

The bottom face button.

var buttonB: GCControllerButtonInput

The right face button.

var buttonX: GCControllerButtonInput

The left face button.

var buttonY: GCControllerButtonInput

The top face button.

### Saving a Snapshot

func saveSnapshot() -> GCGamepadSnapshot

Saves a snapshot of all of the profile’s elements.

### Constants

typealias GCGamepadValueChangedHandler

Signature for the block executed if any element in the gamepad profile changes value.

## Relationships

### Inherits From

- GCPhysicalInputProfile

### Inherited By

- GCGamepadSnapshot

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Deprecated symbols

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

func GCExtendedGamepadSnapshotDataFromNSData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapshotData>?, Data?) -> BoolDeprecated

func GCMicroGamepadSnapshotDataFromNSData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?, Data?) -> BoolDeprecated

func NSDataFromGCExtendedGamepadSnapshotData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapshotData>?) -> Data?Deprecated

func NSDataFromGCMicroGamepadSnapshotData(UnsafeMutablePointer&lt;GCMicroGamepadSnapshotData>?) -> Data?Deprecated

