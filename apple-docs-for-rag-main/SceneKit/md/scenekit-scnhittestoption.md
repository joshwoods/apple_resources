

- SceneKit
-  SCNHitTestOption 

Structure

# SCNHitTestOption

Options affecting the behavior of SceneKit hit-testing methods.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SCNHitTestOption
```

## Topics

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

static let searchMode: SCNHitTestOption

An option for the number and order of hit test results to provide.

enum SCNHitTestSearchMode

Possible values for the searchMode option used with hit-testing methods.

### Deprecated

static let firstFoundOnly: SCNHitTestOption

An option to return only the first object found.

Deprecated

static let sortResults: SCNHitTestOption

An option to sort the results of a hit-test.

Deprecated

### Initializers

init(rawValue: String)

### Type Properties

static let ignoreLightArea: SCNHitTestOption

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Related Documentation

func hitTestWithSegment(from: SCNVector3, to: SCNVector3, options: [String : Any]?) -> [SCNHitTestResult]

Searches the node’s child node subtree for objects intersecting a line segment between two specified points.

### Hit-Testing

func hitTestWithSegment(from: SCNVector3, to: SCNVector3, options: [String : Any]?) -> [SCNHitTestResult]

Searches the node’s child node subtree for objects intersecting a line segment between two specified points.

