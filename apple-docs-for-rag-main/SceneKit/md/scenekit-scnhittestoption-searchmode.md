

- SceneKit
- SCNHitTestOption
-  searchMode 

Type Property

# searchMode

An option for the number and order of hit test results to provide.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
static let searchMode: SCNHitTestOption
```

## Discussion

The value for this key is an NSNumber object containing the raw integer value of an SCNHitTestSearchMode constant.

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

static let rootNode: SCNHitTestOption

The root of the node hierarchy to be searched.

enum SCNHitTestSearchMode

Possible values for the searchMode option used with hit-testing methods.

