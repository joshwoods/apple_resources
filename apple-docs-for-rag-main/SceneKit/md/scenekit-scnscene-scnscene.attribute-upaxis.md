

- SceneKit
- SCNScene
- SCNScene.Attribute
-  upAxis 

Type Property

# upAxis

An `SCNVector3` structure specifying the orientation of the scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let upAxis: SCNScene.Attribute
```

## Discussion

The SCNVector3structure (in an NSValue object) may be present in scenes loaded from scene files produced using external tools, but has no effect on SceneKit’s processing of the scene. Use this vector when combining elements from different scenes so that they appear in their expected orientation.

## See Also

### Type Properties

static let endTime: SCNScene.Attribute

static let frameRate: SCNScene.Attribute

A floating-point value for the frame rate of the scene.

static let startTime: SCNScene.Attribute

