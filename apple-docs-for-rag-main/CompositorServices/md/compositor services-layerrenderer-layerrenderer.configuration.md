

- Compositor Services
- LayerRenderer
-  LayerRenderer.Configuration 

Structure

# LayerRenderer.Configuration

A type that stores the texture formats, layout information, and other details you use to configure your rendering loop code.

visionOS 1.0+

``` source
struct Configuration
```

## Overview

A LayerRenderer.Configuration type stores the configuration options for your app’s LayerRenderer object. When configuring your app’s CompositorLayer type, use this type to specify information about the texture layouts, pixel formats, and rendering options you want. The system uses the provided information to initialize the LayerRenderer object. It also uses the information to create the Metal textures and other data structures that you use for each frame of content.

You don’t create this type directly. When implementing the makeConfiguration(capabilities:configuration:) method of your CompositorLayerConfiguration type, the system passes a set of default configuration values for you to modify.

## Topics

### Configuring the color textures

var colorFormat: MTLPixelFormat

The pixel format to use for color textures.

var colorUsage: MTLTextureUsage

The texture usage value to apply to the layer’s color textures.

### Configuring the depth information

var depthFormat: MTLPixelFormat

The pixel format to use for the layer’s depth textures.

var depthUsage: MTLTextureUsage

The texture usage value to apply to the layer’s depth textures.

var defaultDepthRange: SIMD2&lt;Float>

The distances to the far and near clipping planes that define the bounds of your content.

### Configuring the texture layout

var layout: LayerRenderer.Layout

The layout being used by the layer.

enum Layout

Constants that specify the organization of the textures you use for drawing.

### Configuring the foveation setting

var isFoveationEnabled: Bool

A value that indicates if the layer is using variable rasterization rates.

var generateFlippedRasterizationRateMaps: Bool

A Boolean value that indicates whether the layer renderer provides rasterization rate maps flipped around the y-axis.

## Relationships

### Conforms To

- Copyable

## See Also

### Configuring the layer renderer

var configuration: LayerRenderer.Configuration

The configuration details for the specified layer.

struct Capabilities

The color formats, depth formats, and features that you can use to configure your rendering engine.

