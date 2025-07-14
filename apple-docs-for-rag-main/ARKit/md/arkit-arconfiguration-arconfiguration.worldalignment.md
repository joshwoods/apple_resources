

- ARKit
- ARConfiguration
-  ARConfiguration.WorldAlignment 

Enumeration

# ARConfiguration.WorldAlignment

Options for how ARKit constructs a scene coordinate system based on real-world device motion.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
enum WorldAlignment
```

## Topics

### Alignments

case gravity

The coordinate system’s y-axis is parallel to gravity, and its origin is the initial position of the device.

case gravityAndHeading

The coordinate system’s y-axis is parallel to gravity, its x- and z-axes are oriented to compass heading, and its origin is the initial position of the device.

case camera

The scene coordinate system is locked to match the orientation of the camera.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the AR session

var isLightEstimationEnabled: Bool

A Boolean value specifying whether ARKit analyzes scene lighting in captured camera images.

var worldAlignment: ARConfiguration.WorldAlignment

A value specifying how the session maps real-world device motion into a 3D scene coordinate system.

