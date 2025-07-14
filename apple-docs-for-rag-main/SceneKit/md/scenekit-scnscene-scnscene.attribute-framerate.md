

- SceneKit
- SCNScene
- SCNScene.Attribute
-  frameRate 

Type Property

# frameRate

A floating-point value for the frame rate of the scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let frameRate: SCNScene.Attribute
```

## Discussion

This value (in an NSNumber object) may be present in scenes loaded from scene files produced using external tools, but has no effect on SceneKit’s rendering of the scene.

## See Also

### Type Properties

static let endTime: SCNScene.Attribute

static let startTime: SCNScene.Attribute

static let upAxis: SCNScene.Attribute

An `SCNVector3` structure specifying the orientation of the scene.

