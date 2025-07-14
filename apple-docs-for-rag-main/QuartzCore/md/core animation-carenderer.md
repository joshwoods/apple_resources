

- Core Animation
-  CARenderer 

Class

# CARenderer

A layer that allows an application to render a layer tree into a Core OpenGL context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CARenderer
```

## Overview

For real-time output you should use an instance of NSView to host the layer-tree.

## Topics

### Creating a Renderer

init(cglContext: UnsafeMutableRawPointer, options: [AnyHashable : Any]?)

Creates and returns a `CARenderer` instance with the render target specified by the Core OpenGL context.

init(mtlTexture: any MTLTexture, options: [AnyHashable : Any]?)

Creates a layer renderer from a Metal texture.

### Getting the Rendered Layer

var layer: CALayer?

The root layer of the layer-tree the receiver should render.

### Determining Layer Bounds

var bounds: CGRect

The bounds of the receiver.

### Rendering a Frame

func beginFrame(atTime: CFTimeInterval, timeStamp: UnsafeMutablePointer&lt;CVTimeStamp>?)

Begin rendering a frame at the specified time.

func updateBounds() -> CGRect

Returns the bounds of the update region that contains all pixels that will be rendered by the current frame.

func addUpdate(CGRect)

Adds the rectangle to the update region of the current frame.

func render()

Render the update region of the current frame to the target context.

func nextFrameTime() -> CFTimeInterval

Returns the time at which the next update should happen.

func endFrame()

Release any data associated with the current frame.

### Instance Methods

func setDestination(any MTLTexture)

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

### Metal and OpenGL

class CAMetalLayer

A Core Animation layer that Metal can render into, typically displayed onscreen.

protocol CAMetalDrawable

A Metal drawable associated with a Core Animation layer.

class CAEAGLLayer

A layer that supports drawing OpenGL content in iOS and tvOS applications.

Deprecated

class CAEDRMetadata

Metadata describing how extended dynamic range (EDR) values should be tone mapped.

class CAOpenGLLayer

A layer that provides a layer suitable for rendering OpenGL content.

Deprecated

