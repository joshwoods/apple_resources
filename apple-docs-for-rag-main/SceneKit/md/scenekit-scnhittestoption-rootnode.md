

- SceneKit
- SCNHitTestOption
-  rootNode 

Type Property

# rootNode

The root of the node hierarchy to be searched.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let rootNode: SCNHitTestOption
```

## Discussion

The value for this key is an SCNNode object. Hit-testing searches only the child node hierarchy under this node. When hit-testing takes place in the screen space of an SCNSceneRenderer object with the hitTest(_:options:) method, the default value is the presented scene’s root node. When hit-testing is in a node using its hitTestWithSegment(from:to:options:), the default value is the node.

## See Also

### Options

static let backFaceCulling: SCNHitTestOption

An option to ignore faces not oriented toward the camera.

static let boundingBoxOnly: SCNHitTestOption

An option to search for objects by bounding box only.

static let categoryBitMask: SCNHitTestOption

An option to search only for objects matching a specified bitmask.

static let clipToZRange: SCNHitTestOption

An option to search for objects only within the depth range of the current point of view.

static let ignoreChildNodes: SCNHitTestOption

An option to ignore child nodes when searching.

static let ignoreHiddenNodes: SCNHitTestOption

An option to ignore hidden nodes when searching.

static let searchMode: SCNHitTestOption

An option for the number and order of hit test results to provide.

enum SCNHitTestSearchMode

Possible values for the searchMode option used with hit-testing methods.

