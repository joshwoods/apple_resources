

- RealityKit
- ARView
-  ARView.CameraMode 

Enumeration

# ARView.CameraMode

The available camera modes.

iOSiPadOSMac Catalyst

``` source
enum CameraMode
```

## Topics

### Setting the camera mode

case ar

Use the device’s camera, managed by the AR session.

case nonAR

Use the device’s camera, managed by the AR session.

### Comparing modes

static func == (ARView.CameraMode, ARView.CameraMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Camera mode settings

struct RealityViewCamera

A camera for reality view scenes, that can be world tracking or virtual.

struct CameraControls

