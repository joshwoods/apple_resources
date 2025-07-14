

- AppKit
- NSOpenGLContext
-  NSOpenGLContext.Parameter Deprecated

Enumeration

# NSOpenGLContext.Parameter

Constants that specify context parameters.

macOS 10.0–10.14Deprecated

``` source
enum Parameter
```

Deprecated

OpenGL API deprecated; please use Metal and MetalKit. (Define GL_SILENCE_DEPRECATION to silence these warnings.)

## Overview

These attribute names are used by setValues(_:for:) and getValues(_:for:).

## Topics

### Parameters

case swapInterval

Set or get the swap interval.

case surfaceOrder

Set or get the surface order.

case surfaceOpacity

Set or get the surface opacity.

case surfaceBackingSize

Set or get the height and width of the back buffer.

case reclaimResources

Enable or disable reclaiming resources.

case currentRendererID

Get the current renderer ID.

case gpuVertexProcessing

Get whether the CPU is currently processing vertices with the GPU.

case gpuFragmentProcessing

Get whether the CPU is currently processing fragments with the GPU.

case hasDrawable

Returns a Boolean that indicates whether a drawable is attached to the context.

case mpSwapsInFlight

The number of frames that the multithreaded OpenGL engine can process before stalling.

case swapRectangle

Sets or gets the swap rectangle.

case swapRectangleEnable

Enables or disables the swap rectangle in the context’s drawable object.

case rasterizationEnable

If disabled, all rasterization of 2D and 3D primitives is disabled.

case stateValidation

If enabled, OpenGL inspects the context state each time the update method is called to ensure that it is in an appropriate state for switching between renderers.

case surfaceSurfaceVolatile

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

