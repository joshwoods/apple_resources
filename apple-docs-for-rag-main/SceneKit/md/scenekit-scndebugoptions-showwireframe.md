

- SceneKit
- SCNDebugOptions
-  showWireframe 

Type Property

# showWireframe

Display geometries in the scene with wireframe rendering.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var showWireframe: SCNDebugOptions { get }
```

## Discussion

When this option is enabled, SceneKit still renders scene geometry with all associated materials, then overlays a wireframe rendering of the same geometry. You can use this option, for example, to debug material rendering issues.

## See Also

### Debugging Geometry and Animation

static var showBoundingBoxes: SCNDebugOptions

Display the bounding boxes for any nodes with content.

static var renderAsWireframe: SCNDebugOptions

Display only wireframe placeholders for geometries in the scene.

static var showSkeletons: SCNDebugOptions

Display visualizations of the skeletal animation parameters for relevant geometries.

static var showCreases: SCNDebugOptions

Display nonsmoothed crease regions for geometries affected by surface subdivision.

static var showConstraints: SCNDebugOptions

Display visualizations of the constraint objects acting on nodes in the scene.

