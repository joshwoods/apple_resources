

- SceneKit
- SCNHitTestOption
-  clipToZRange 

Type Property

# clipToZRange

An option to search for objects only within the depth range of the current point of view.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let clipToZRange: SCNHitTestOption
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value. The default value is true, specifying that hit-testing searches only objects between the zNear and zFar distances of the pointOfView camera. Specify false to include objects outside this depth range in the search.

This option is valid only when hit-testing in the screen space of an SCNSceneRenderer object with the hitTest(_:options:) method.

## See Also

### Options

static let backFaceCulling: SCNHitTestOption

An option to ignore faces not oriented toward the camera.

static let boundingBoxOnly: SCNHitTestOption

An option to search for objects by bounding box only.

static let categoryBitMask: SCNHitTestOption

An option to search only for objects matching a specified bitmask.

static let ignoreChildNodes: SCNHitTestOption

An option to ignore child nodes when searching.

static let ignoreHiddenNodes: SCNHitTestOption

An option to ignore hidden nodes when searching.

static let rootNode: SCNHitTestOption

The root of the node hierarchy to be searched.

static let searchMode: SCNHitTestOption

An option for the number and order of hit test results to provide.

enum SCNHitTestSearchMode

Possible values for the searchMode option used with hit-testing methods.

