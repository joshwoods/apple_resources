

- SceneKit
- SCNDebugOptions
-  renderAsWireframe 

Type Property

# renderAsWireframe

Display only wireframe placeholders for geometries in the scene.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
static var renderAsWireframe: SCNDebugOptions { get }
```

## Discussion

Unlike the showWireframe option, this option disables normal surface rendering, displaying only the wireframe for each geometry.

## See Also

### Debugging Geometry and Animation

static var showBoundingBoxes: SCNDebugOptions

Display the bounding boxes for any nodes with content.

static var showWireframe: SCNDebugOptions

Display geometries in the scene with wireframe rendering.

static var showSkeletons: SCNDebugOptions

Display visualizations of the skeletal animation parameters for relevant geometries.

static var showCreases: SCNDebugOptions

Display nonsmoothed crease regions for geometries affected by surface subdivision.

static var showConstraints: SCNDebugOptions

Display visualizations of the constraint objects acting on nodes in the scene.

