

- ARKit
- ARConfiguration
-  isLightEstimationEnabled 

Instance Property

# isLightEstimationEnabled

A Boolean value specifying whether ARKit analyzes scene lighting in captured camera images.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var isLightEstimationEnabled: Bool { get set }
```

## Discussion

When this value is true (the default), a running AR session provides scene lighting information in the lightEstimate property of each ARFrame object it captures.

If you render your own overlay graphics for the AR scene, you can use this information in shading algorithms to help make those graphics match the real-world lighting conditions of the scene captured by the camera. (The ARSCNView class automatically uses this information to configure SceneKit lighting.)

## See Also

### Configuring the AR session

var worldAlignment: ARConfiguration.WorldAlignment

A value specifying how the session maps real-world device motion into a 3D scene coordinate system.

enum WorldAlignment

Options for how ARKit constructs a scene coordinate system based on real-world device motion.

