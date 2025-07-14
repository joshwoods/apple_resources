

- SceneKit
- SCNHitTestOption
-  ignoreChildNodes 

Type Property

# ignoreChildNodes

An option to ignore child nodes when searching.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let ignoreChildNodes: SCNHitTestOption
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value. The default value is false, specifying that hit-testing may return objects from any portion of the node hierarchy. Specify true to search only the node specified by the rootNode key.

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

static let ignoreHiddenNodes: SCNHitTestOption

An option to ignore hidden nodes when searching.

static let rootNode: SCNHitTestOption

The root of the node hierarchy to be searched.

static let searchMode: SCNHitTestOption

An option for the number and order of hit test results to provide.

enum SCNHitTestSearchMode

Possible values for the searchMode option used with hit-testing methods.

