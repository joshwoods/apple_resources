

- Compositor Services
- LayerRenderer
- LayerRenderer.Drawable
-  LayerRenderer.Drawable.View 

Structure

# LayerRenderer.Drawable.View

A type that provides information on how to render content into the frame’s textures.

visionOS 1.0+

``` source
struct View
```

## Overview

Compositor Services provides a view for each distinct render viewpoint. For example, a head-mounted display typically contains two views: one for each eye. Use the information in the views to set up your render pass descriptor, or to determine which part of a texture to fill with content.

## Topics

### Getting the view’s texture map

var textureMap: LayerRenderer.Drawable.View.TextureMap

The texture map for a view.

struct TextureMap

A type that provides details about the textures associated with a view.

### Getting the transformations

var transform: simd_float4x4

The transformation matrix that converts between the device’s coordinate space to the position of the view in that space.

var tangents: simd_float4

The tangent values for the angles you use to determine the planes of the viewing frustum.

Deprecated

### Creating a view

init()

Creates a view type.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Drawing environment

struct Drawable

A type that provides the textures and information you need to draw a frame of content.

