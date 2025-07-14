

- RealityKit
-  CameraControls 

Structure

# CameraControls

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct CameraControls
```

## Topics

### Operators

static func == (CameraControls, CameraControls) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static var dolly: CameraControls

Move the camera forward and backward by dragging a trackpad or mouse.

static var none: CameraControls

Disable camera control via gestures.

static var orbit: CameraControls

Move the camera around a target by dragging a trackpad or mouse.

static var pan: CameraControls

Move the viewport up, left, right, or down by dragging a trackpad or mouse.

static var tilt: CameraControls

Change the viewing angle by dragging a trackpad or mouse.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Camera mode settings

struct RealityViewCamera

A camera for reality view scenes, that can be world tracking or virtual.

enum CameraMode

The available camera modes.

