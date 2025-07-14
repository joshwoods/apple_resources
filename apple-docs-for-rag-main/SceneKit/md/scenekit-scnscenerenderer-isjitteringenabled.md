

- SceneKit
- SCNSceneRenderer
-  isJitteringEnabled 

Instance Property

# isJitteringEnabled

A Boolean value that determines whether SceneKit applies jittering to reduce aliasing artifacts.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isJitteringEnabled: Bool { get set }
```

**Required**

## Discussion

Jittering is a process that SceneKit uses to improve the visual quality of a rendered scene. While the scene’s content is still, SceneKit moves the pointOfView location very slightly (by less than a pixel in projected screen space). It then composites images rendered after several such moves to create the final rendered scene, creating an antialiasing effect that smooths the edges of rendered geometry.

By default, the value of this property is false, specifying that SceneKit should not perform jittering. Change the value to true to enable jittering.

Because the SCNView and SCNLayer classes perform jittering automatically and asynchronously, enabling jittering for these classes has minimal impact on rendering performance. The SCNRenderer class performs jittering synchronously, incurring a high performance cost. With this class, jittering is suitable for rendering single frames on demand, but not for real-time rendering.

## See Also

### Managing Scene Display

var pointOfView: SCNNode?

The node from which the scene’s contents are viewed for rendering.

**Required**

var autoenablesDefaultLighting: Bool

A Boolean value that determines whether SceneKit automatically adds lights to a scene.

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

