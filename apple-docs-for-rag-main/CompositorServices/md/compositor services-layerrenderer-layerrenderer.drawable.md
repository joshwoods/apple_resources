

- Compositor Services
- LayerRenderer
-  LayerRenderer.Drawable 

Structure

# LayerRenderer.Drawable

A type that provides the textures and information you need to draw a frame of content.

visionOS 1.0+

``` source
struct Drawable
```

## Mentioned in 

Drawing fully immersive content using Metal

## Overview

When you draw a frame of content, the frame’s LayerRenderer.Drawable type provides the actual textures and rendering information you need. Do as much work as possible in advance to prepare for rendering, and retrieve the LayerRenderer.Drawable only when you’re ready to start encoding commands into your Metal command buffers. The system recycles frames and their drawables for efficiency, so if you retrieve the drawable too early, it might not be ready to use.

Use the drawable’s LayerRenderer.Drawable.View instances to determine where to draw your content in the provided textures. After you finish encoding your content, call encodePresent(commandBuffer:) to add a presentation notification to your command buffer. This command tells Compositor Services when to display the frame, and is essential for displaying your frame on time.

## Topics

### Getting the views

var views: [LayerRenderer.Drawable.View]

An array of viewports that tell you how to draw to the drawable’s textures

struct View

A type that provides information on how to render content into the frame’s textures.

### Accessing the device orientation

var deviceAnchor: DeviceAnchor?

The device position and orientation you used to render the frame.

### Getting the render textures

var colorTextures: [any MTLTexture]

An array of color textures to use to render the current frame.

var depthTextures: [any MTLTexture]

An array of depth textures to use to render the current frame.

### Enqueueing a command buffer

func encodePresent(commandBuffer: any MTLCommandBuffer)

Encodes a notification event to the specified command buffer to present the drawable’s content onscreen.

### Getting the rasterization rate map

var rasterizationRateMaps: [any MTLRasterizationRateMap]

The rasterization rate maps to use when rendering the frame.

var flippedRasterizationRateMaps: [any MTLRasterizationRateMap]

The rasterization rate maps that are flipped around the y-axis.

### Getting the projection matrix

enum AxisDirectionConvention

Constants that indicate the axis and direction to use for a perspective projection matrix.

### Accessing pixel depth information

var depthRange: simd_float2

The distances to the far and near clipping planes from the person viewing the content, in meters.

### Managing the state machine

var state: LayerRenderer.Drawable.State

The current operational state of a drawable instance.

enum State

The state of ownership for the drawable.

### Synchronizing the drawing operation

var frameTiming: LayerRenderer.Frame.Timing

The timing information for the drawable’s frame.

var presentationFrameIndex: CompositorFrameIndex

The sequential index of a drawable’s frame.

### Creating a drawable

init()

Creates an uninitialized drawable.

### Instance Methods

func computeProjection(convention: AxisDirectionConvention, viewIndex: Int) -> matrix_float4x4

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Drawing environment

struct View

A type that provides information on how to render content into the frame’s textures.

