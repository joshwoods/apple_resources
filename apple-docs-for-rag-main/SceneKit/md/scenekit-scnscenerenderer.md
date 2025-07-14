

- SceneKit
-  SCNSceneRenderer 

Protocol

# SCNSceneRenderer

Methods and properties common to the SCNView, SCNLayer, and SCNRenderer classes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol SCNSceneRenderer : NSObjectProtocol
```

## Overview

You use an instance of one of these classes to display a scene and manage SceneKit’s rendering and animation of the scene’s contents.

Typically, you use the SCNView class to display a scene in a window (or full screen). You can create and configure a SceneKit view programmatically or in Interface Builder. The other renderer classes render SceneKit content in more specialized situations. If your app has a user interface composed of Core Animation layers, you can use the SCNLayer class to render a scene into a layer. If your app uses Metal or OpenGL for other rendering, you can use the SCNRenderer class to render SceneKit content with the same Metal device or OpenGL context.

Use the scene property of the view, layer, or renderer to specify the scene to display.

## Topics

### Presenting a Scene

var scene: SCNScene?

The scene to be displayed.

**Required**

func present(SCNScene, with: SKTransition, incomingPointOfView: SCNNode?, completionHandler: (() -> Void)?)

Displays the specified scene with an animated transition.

**Required**

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

var renderingAPI: SCNRenderingAPI

The graphics technology SceneKit uses to render the scene.

**Required**

struct SCNDebugOptions

Options for drawing overlays with SceneKit content that can aid in debugging, used with the debugOptions property.

enum SCNRenderingAPI

Options for choosing the graphics technology for an SCNView object (or other SceneKit renderer) to use for drawing its contents. Used by the renderingAPI property and the preferredRenderingAPI option when initializing an SCNView object.

### Managing Scene Animation Timing

var sceneTime: TimeInterval

The current scene time.

**Required**

var isPlaying: Bool

A Boolean value that determines whether the scene is playing.

**Required**

var loops: Bool

A Boolean value that determines whether SceneKit restarts the scene time after all animations in the scene have played.

**Required**

### Preloading Renderer Resources

func prepare(Any, shouldAbortBlock: (() -> Bool)?) -> Bool

Prepares a SceneKit object for rendering.

**Required**

func prepare([Any], completionHandler: ((Bool) -> Void)?)

Prepares the specified SceneKit objects for rendering, using a background thread.

**Required**

### Working With Projected Scene Contents

func hitTest(CGPoint, options: [SCNHitTestOption : Any]?) -> [SCNHitTestResult]

Searches the renderer’s scene for objects corresponding to a point in the rendered image.

**Required**

struct SCNHitTestOption

Options affecting the behavior of SceneKit hit-testing methods.

func isNode(SCNNode, insideFrustumOf: SCNNode) -> Bool

Returns a Boolean value indicating whether a node might be visible from a specified point of view.

**Required**

func nodesInsideFrustum(of: SCNNode) -> [SCNNode]

Returns all nodes that might be visible from a specified point of view.

**Required**

func projectPoint(SCNVector3) -> SCNVector3

Projects a point from the 3D world coordinate system of the scene to the 2D pixel coordinate system of the renderer.

**Required**

func unprojectPoint(SCNVector3) -> SCNVector3

Unprojects a point from the 2D pixel coordinate system of the renderer to the 3D world coordinate system of the scene.

**Required**

### Participating in the Scene Rendering Process

var delegate: (any SCNSceneRendererDelegate)?

A delegate object that receives messages about SceneKit’s rendering process.

**Required**

### Customizing Scene Rendering with Metal

var currentRenderCommandEncoder: (any MTLRenderCommandEncoder)?

The Metal render command encoder in use for the current SceneKit rendering pass.

**Required**

var device: (any MTLDevice)?

The Metal device this renderer uses for rendering.

**Required**

var commandQueue: (any MTLCommandQueue)?

The Metal command queue this renderer uses for rendering.

**Required**

var colorPixelFormat: MTLPixelFormat

The Metal pixel format for the renderer’s color output.

**Required**

var depthPixelFormat: MTLPixelFormat

The Metal pixel format for the renderer’s depth buffer.

**Required**

var stencilPixelFormat: MTLPixelFormat

The Metal pixel format for the renderer’s stencil buffer.

**Required**

### Customizing Scene Rendering with OpenGL

var context: UnsafeMutableRawPointer?

The OpenGL rendering context that SceneKit uses for rendering the scene.

**Required**

### Rendering Sprite Kit Content over a Scene

var overlaySKScene: SKScene?

A Sprite Kit scene to be rendered on top of the SceneKit content.

**Required**

### Working With Positional Audio

var audioListener: SCNNode?

The node representing the listener’s position in the scene for use with positional audio effects.

**Required**

var audioEnvironmentNode: AVAudioEnvironmentNode

The 3D audio mixing node SceneKit uses for positional audio effects.

**Required**

var audioEngine: AVAudioEngine

The audio engine SceneKit uses for playing scene sounds.

**Required**

### Instance Properties

var currentRenderPassDescriptor: MTLRenderPassDescriptor

**Required**

var currentTime: TimeInterval

**Required**

Deprecated

var currentViewport: CGRect

**Required**

var isTemporalAntialiasingEnabled: Bool

**Required**

var usesReverseZ: Bool

**Required**

var workingColorSpace: CGColorSpace

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- SCNLayer
- SCNRenderer
- SCNView

## See Also

### Display and Interactivity

protocol SCNSceneRendererDelegate

Methods your app can implement to participate in SceneKit’s animation loop or perform additional rendering.

class SCNLayer

A Core Animation layer that renders a SceneKit scene as its content.

Deprecated

class SCNRenderer

A renderer for displaying a SceneKit scene in an existing Metal workflow or OpenGL context.

class SCNHitTestResult

Information about the result of a scene-space or view-space search for scene elements.

