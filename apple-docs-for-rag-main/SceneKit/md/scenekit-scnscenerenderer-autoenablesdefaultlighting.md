

- SceneKit
- SCNSceneRenderer
-  autoenablesDefaultLighting 

Instance Property

# autoenablesDefaultLighting

A Boolean value that determines whether SceneKit automatically adds lights to a scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var autoenablesDefaultLighting: Bool { get set }
```

**Required**

## Discussion

If this property’s value is false (the default), the only light sources SceneKit uses for rendering a scene are those contained in the scene graph. If you change the value to true, SceneKit automatically adds and places an omnidirectional light source when rendering scenes that contain no lights or only contain ambient lights.

## See Also

### Managing Scene Display

var pointOfView: SCNNode?

The node from which the scene’s contents are viewed for rendering.

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

