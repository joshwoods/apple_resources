

- SceneKit
- SCNSceneRenderer
-  debugOptions 

Instance Property

# debugOptions

Options for drawing overlay content in a scene that can aid debugging.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var debugOptions: SCNDebugOptions { get set }
```

**Required**

## Discussion

Use these options to display overlays that show otherwise-invisible scene content—such as node bounding boxes and the extents of physics fields—for use in debugging and profiling your app. For example:

- To visualize how well each object’s physics representation corresponds to its visible geometry, show the shape of each SCNPhysicsBody object in the scene with the showPhysicsShapes option.

- To improve rendering performance in a scene with multiple SCNLight objects, show each light’s area of effect with the showLightExtents option and ensure that each object in the scene is affected by no more than three lights.

## See Also

### Managing Scene Display

var pointOfView: SCNNode?

The node from which the scene’s contents are viewed for rendering.

**Required**

var autoenablesDefaultLighting: Bool

A Boolean value that determines whether SceneKit automatically adds lights to a scene.

**Required**

var isJitteringEnabled: Bool

A Boolean value that determines whether SceneKit applies jittering to reduce aliasing artifacts.

**Required**

var showsStatistics: Bool

A Boolean value that determines whether SceneKit displays rendering performance statistics in an accessory view.

**Required**

var renderingAPI: SCNRenderingAPI

The graphics technology SceneKit uses to render the scene.

**Required**

struct SCNDebugOptions

Options for drawing overlays with SceneKit content that can aid in debugging, used with the debugOptions property.

enum SCNRenderingAPI

Options for choosing the graphics technology for an SCNView object (or other SceneKit renderer) to use for drawing its contents. Used by the renderingAPI property and the preferredRenderingAPI option when initializing an SCNView object.

