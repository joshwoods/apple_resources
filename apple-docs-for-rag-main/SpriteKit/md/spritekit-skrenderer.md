

- SpriteKit
-  SKRenderer 

Class

# SKRenderer

An object that renders a scene into a custom Metal rendering pipeline and drives the scene update cycle.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class SKRenderer
```

## Mentioned in 

Choosing a SpriteKit Scene Renderer

## Overview

SKRenderer allows an app to mix SpriteKit and Metal content by rendering an SKScene into a Metal command buffer. The reasons an app may do this instead of displaying a scene in SKView are:

1.  Apps that are built in Metal can mix in SpriteKit content. While it’s possible to add SKView as a subview to a Metal view, plugging SKRenderer into their Metal pipeline allows layering SpriteKit content at a specific z-position.

2.  You might be writing a SpriteKit app and decide later to take full control over some portion of renderering by implementing it with Metal, yet continue to use SpriteKit for the rest of the app. For example, you might write the environmental effects layer of your app that does fog, clouds, and rain, with custom Metal shaders, and continue to layer content below and above that with SpriteKit.

## Topics

### First Steps

Create a renderer by specifying a GPU and then set its scene.

init(device: any MTLDevice)

Initializes with a specific GPU to render into.

var scene: SKScene?

The scene this renderer will draw into the Metal command buffer.

### Rendering the Scene

Draw the renderer’s scene into a custom Metal rendering pipeline.

func render(withViewport: CGRect, commandBuffer: any MTLCommandBuffer, renderPassDescriptor: MTLRenderPassDescriptor)

func render(withViewport: CGRect, renderCommandEncoder: any MTLRenderCommandEncoder, renderPassDescriptor: MTLRenderPassDescriptor, commandQueue: any MTLCommandQueue)

### Driving the Scene’s Update Cycle

Control when the scene’s delegate functions are called.

func update(atTime: TimeInterval)

### Configuring Performance Related Toggles

Control hints that have performance implications which are unique to your app.

var ignoresSiblingOrder: Bool

var shouldCullNonVisibleNodes: Bool

### Enabling Visual Statistics for Debugging

Display metrics in the bottom corner of the scene’s frame for debugging purposes.

var showsNodeCount: Bool

A Boolean value that indicates whether the view displays an overlay that shows physics bodies that are visible in the scene.

var showsDrawCount: Bool

A Boolean value that indicates whether the view displays the number of drawing passes it needed to render the view.

var showsQuadCount: Bool

A Boolean value that indicates whether the view displays the number of rectangles used to render the scene.

var showsPhysics: Bool

A Boolean value that indicates whether the view displays physics-related debugging information.

var showsFields: Bool

A Boolean value that indicates whether the view displays information about physics fields in the scene.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Scene Renderers

Choosing a SpriteKit Scene Renderer

Compare the different ways to display a SpriteKit scene.

class SKView

A view subclass that renders a SpriteKit scene.

class WKInterfaceSKScene

A visual WatchKit element that displays a SpriteKit scene.

