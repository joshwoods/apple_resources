

- SceneKit
- SCNDebugOptions
-  showWorldOrigin 

Type Property

# showWorldOrigin

Display a coordinate axis visualization indicating the position and orientation of the AR world coordinate system.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static let showWorldOrigin: SCNDebugOptions
```

## Discussion

This visualization is available to all session configurations and session worldAlignment options, but is most useful with a ARWorldTrackingConfiguration session. For example, if you start running a session when this option is enabled, then take a step backward, the real-world position tracked by the AR world coordinate system should become visible on your device screen.

