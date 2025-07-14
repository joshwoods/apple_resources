

- DockKit
- DockAccessory
-  DockAccessory.CameraOrientation 

Enumeration

# DockAccessory.CameraOrientation

The set of camera orientations used to extract coordinates.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
enum CameraOrientation
```

## Topics

### Getting camera orientation

case corrected

The orientation corresponds to the unit rectangle.

case faceUp

The orientation is facing up.

case faceDown

The orientation is facing down.

case landscapeLeft

The orientation is landscape left.

case landscapeRight

The orientation is landscape right.

case portrait

The orientation is portrait.

case portraitUpsideDown

The orientation is portrait, upside down.

case unknown

The orientation is unknown.

### Operators

static func == (DockAccessory.CameraOrientation, DockAccessory.CameraOrientation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Selecting and tracking

func selectSubject(at: CGPoint) async throws

Selects a subject to track at the supplied coordinates.

func track([AVMetadataObject], cameraInformation: DockAccessory.CameraInformation) async throws

Automatically generate and send tracking vectors to the device.

func track([DockAccessory.Observation], cameraInformation: DockAccessory.CameraInformation) async throws

Automatically generate and send tracking vectors to the device.

struct Observation

An observation of the contents of a single video frame.

struct CameraInformation

A collection of tracking information about the camera currently in use.

