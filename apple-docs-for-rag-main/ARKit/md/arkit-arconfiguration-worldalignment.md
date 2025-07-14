

- ARKit
- ARConfiguration
-  worldAlignment 

Instance Property

# worldAlignment

A value specifying how the session maps real-world device motion into a 3D scene coordinate system.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var worldAlignment: ARConfiguration.WorldAlignment { get set }
```

## Mentioned in 

Understanding World Tracking

## Discussion

Creating an AR experience depends on being able to construct a coordinate system for placing objects in a virtual 3D world that maps to the real-world position and motion of the device. When you run a session configuration, ARKit creates a scene coordinate system based on the position and orientation of the device; any ARAnchor objects you create or that the AR session detects are positioned relative to that coordinate system.

See ARConfiguration.WorldAlignment for possible values.

## See Also

### Configuring the AR session

var isLightEstimationEnabled: Bool

A Boolean value specifying whether ARKit analyzes scene lighting in captured camera images.

enum WorldAlignment

Options for how ARKit constructs a scene coordinate system based on real-world device motion.

