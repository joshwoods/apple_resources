

- Compositor Services
- LayerRenderer
- LayerRenderer.Drawable
- LayerRenderer.Drawable.View
-  LayerRenderer.Drawable.View.TextureMap 

Structure

# LayerRenderer.Drawable.View.TextureMap

A type that provides details about the textures associated with a view.

visionOS 1.0+

``` source
struct TextureMap
```

## Overview

A texture map helps you locate the content for a specific view within a texture. Texture maps are especially important when a layer uses a single texture to manage multiple views. For example, a head-mounted display might store the images for both the left and right eyes in a single texture. Pass this type to other functions to get specific details about the current texture, such as its view bounds or its index into a texture array.

## Topics

### Getting the viewport

var viewport: MTLViewport

The portion of the texture that the view uses to draw its content.

### Getting the texture indices

var sliceIndex: Int

The index of the view’s texture in an array-based texture type.

var textureIndex: Int

The index of the view’s textures in the drawable.

### Creating a texture map

init()

Creates an uninitialized texture map.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Getting the view’s texture map

var textureMap: LayerRenderer.Drawable.View.TextureMap

The texture map for a view.

