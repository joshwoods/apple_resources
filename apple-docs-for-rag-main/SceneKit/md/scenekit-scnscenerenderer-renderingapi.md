

- SceneKit
- SCNSceneRenderer
-  renderingAPI 

Instance Property

# renderingAPI

The graphics technology SceneKit uses to render the scene.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var renderingAPI: SCNRenderingAPI { get }
```

**Required**

## Discussion

You choose a graphics technology when initializing a scene renderer:

- When initializing a SCNView object, use the init(frame:options:) initializer and the preferredRenderingAPI key. Alternatively, create a view in Interface Builder and use the Rendering API control in the inspector. During initialization, the view will attempt to use the preferred API, but will fall back to a different API if the preferred one is not supported on the current hardware.

- To create a SCNRenderer object that renders into your own OpenGL contect, use the init(context:options:) initializer. To create a renderer for use in your own Metal workflow, use the init(device:options:) initializer.

- The rendering technology used by a SCNLayer object is determined by Core Animation.

After initializing a renderer, this property reflects the rendering technology in use.

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

var debugOptions: SCNDebugOptions

Options for drawing overlay content in a scene that can aid debugging.

**Required**

struct SCNDebugOptions

Options for drawing overlays with SceneKit content that can aid in debugging, used with the debugOptions property.

enum SCNRenderingAPI

Options for choosing the graphics technology for an SCNView object (or other SceneKit renderer) to use for drawing its contents. Used by the renderingAPI property and the preferredRenderingAPI option when initializing an SCNView object.

