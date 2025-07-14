

- SceneKit
- SCNHitTestOption
-  ignoreHiddenNodes 

Type Property

# ignoreHiddenNodes

An option to ignore hidden nodes when searching.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
static let ignoreHiddenNodes: SCNHitTestOption
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value. The default value is true, specifying that hit-testing should not return nodes whose hidden property value is true. Specify false to search nodes regardless of their visibility.

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

static let rootNode: SCNHitTestOption

The root of the node hierarchy to be searched.

static let searchMode: SCNHitTestOption

An option for the number and order of hit test results to provide.

enum SCNHitTestSearchMode

Possible values for the searchMode option used with hit-testing methods.

