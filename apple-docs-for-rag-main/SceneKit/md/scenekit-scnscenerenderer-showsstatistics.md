

- SceneKit
- SCNSceneRenderer
-  showsStatistics 

Instance Property

# showsStatistics

A Boolean value that determines whether SceneKit displays rendering performance statistics in an accessory view.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var showsStatistics: Bool { get set }
```

**Required**

## Discussion

The SceneKit statistics view displays various information about scene rendering performance and GPU resource usage, including a frames-per-second (fps) counter. In macOS, click the gear button in the statistics view to show a panel with additional controls for adjusting SceneKit’s rendering of the scene.

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

