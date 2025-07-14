

- SceneKit
- SCNDebugOptions
-  showLightExtents 

Type Property

# showLightExtents

Display the regions affected by each SCNLight object in the scene.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var showLightExtents: SCNDebugOptions { get }
```

## Discussion

Only lights whose type is omni or spot have an area of effect; directional and ambient lights affect the entire scene.

## See Also

### Debugging Cameras and Lighting

static var showCameras: SCNDebugOptions

Display visualizations for nodes in the scene with attached cameras and their fields of view.

static var showLightInfluences: SCNDebugOptions

Display the locations of each SCNLight object in the scene.

