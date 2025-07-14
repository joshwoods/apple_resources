

- ARKit
- ARWorldTrackingConfiguration
-  supportsSceneReconstruction(\_:) 

Type Method

# supportsSceneReconstruction(\_:)

Checks if the device supports scene reconstruction.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
class func supportsSceneReconstruction(_ sceneReconstruction: ARConfiguration.SceneReconstruction) -> Bool
```

## Discussion

Scene reconstruction requires a device with a LiDAR Scanner, such as the fourth-generation iPad Pro.

## See Also

### Tracking Surfaces

var planeDetection: ARWorldTrackingConfiguration.PlaneDetection

The configuration’s plane detection options.

struct PlaneDetection

Options for whether and how the framework detects flat surfaces in captured images.

var sceneReconstruction: ARConfiguration.SceneReconstruction

A flag that enables scene reconstruction.

