

- SceneKit
-  SCNRenderer 

Class

# SCNRenderer

A renderer for displaying a SceneKit scene in an existing Metal workflow or OpenGL context.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
class SCNRenderer
```

## Overview

Use this class when you want to add content rendered by SceneKit to an app that already renders other content by using Metal, OpenGL, or OpenGL ES directly. To provide content for a SceneKit renderer, assign a SCNScene object to its scene property.

For additional important methods and properties for working with SceneKit renderers, see SCNSceneRenderer.

## Topics

### Creating a Renderer

convenience init(device: (any MTLDevice)?, options: [AnyHashable : Any]?)

Creates a renderer with the specified Metal device.

convenience init(context: EAGLContext?, options: [AnyHashable : Any]?)

Creates a renderer with the specified OpenGL context.

### Specifying a Scene

var scene: SCNScene?

The scene to be rendered.

### Managing Animation Timing

var nextFrameTime: CFTimeInterval

The timestamp for the next frame to be rendered.

### Rendering a Scene Using Metal

func render(atTime: CFTimeInterval, viewport: CGRect, commandBuffer: any MTLCommandBuffer, passDescriptor: MTLRenderPassDescriptor)

Renders the scene’s contents at the specified system time in the specified Metal command buffer.

### Rendering a Scene Using OpenGL

func render()

Renders the scene’s contents in the renderer’s OpenGL context.

Deprecated

func render(atTime: CFTimeInterval)

Renders the scene’s contents at the specified system time in the renderer’s OpenGL context.

### Capturing a Snapshot

func snapshot(atTime: CFTimeInterval, with: CGSize, antialiasingMode: SCNAntialiasingMode) -> UIImage

Creates an image by drawing the renderer’s content at the specified system time.

### Instance Methods

func render(withViewport: CGRect, commandBuffer: any MTLCommandBuffer, passDescriptor: MTLRenderPassDescriptor)

func update(atTime: CFTimeInterval)

func updateProbes([SCNNode], atTime: CFTimeInterval)

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
- SCNSceneRenderer
- SCNTechniqueSupport

## See Also

### Display and Interactivity

protocol SCNSceneRenderer

Methods and properties common to the SCNView, SCNLayer, and SCNRenderer classes.

protocol SCNSceneRendererDelegate

Methods your app can implement to participate in SceneKit’s animation loop or perform additional rendering.

class SCNLayer

A Core Animation layer that renders a SceneKit scene as its content.

Deprecated

class SCNHitTestResult

Information about the result of a scene-space or view-space search for scene elements.

