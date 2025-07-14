

- SceneKit
- SCNSceneRenderer
-  pointOfView 

Instance Property

# pointOfView

The node from which the scene’s contents are viewed for rendering.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var pointOfView: SCNNode? { get set }
```

**Required**

## Discussion

Use a node with an SCNCamera instance assigned to its camera property to view a scene. The node provides the position and direction of a virtual camera, and the camera object provides rendering parameters such as field of view and focus.

For debugging lights and shadows, you can also designate a spotlight (an SCNLight object whose type property is spot) as a point of view. In this case, the light’s spotInnerAngle property determines the field of view, and its zNear and zFar properties determine the near and far extents of the region that is visible onscreen (also known as the *viewing frustum*).

In either case, the direction of view is along the negative z-axis of the node’s local coordinate space.

## See Also

### Managing Scene Display

var autoenablesDefaultLighting: Bool

A Boolean value that determines whether SceneKit automatically adds lights to a scene.

**Required**

var isJitteringEnabled: Bool

A Boolean value that determines whether SceneKit applies jittering to reduce aliasing artifacts.

**Required**

var showsStatistics: Bool

A Boolean value that determines whether SceneKit displays rendering performance statistics in an accessory view.

**Required**

var debugOptions: SCNDebugOptions

Options for drawing overlay content in a scene that can aid debugging.

**Required**

var renderingAPI: SCNRenderingAPI

The graphics technology SceneKit uses to render the scene.

**Required**

struct SCNDebugOptions

Options for drawing overlays with SceneKit content that can aid in debugging, used with the debugOptions property.

enum SCNRenderingAPI

Options for choosing the graphics technology for an SCNView object (or other SceneKit renderer) to use for drawing its contents. Used by the renderingAPI property and the preferredRenderingAPI option when initializing an SCNView object.

