

- Compositor Services
- LayerRenderer
-  LayerRenderer.Capabilities 

Structure

# LayerRenderer.Capabilities

The color formats, depth formats, and features that you can use to configure your rendering engine.

visionOS 1.0+

``` source
struct Capabilities
```

## Overview

A LayerRenderer.Capabilities type provides information about the capabilities of the current device. Simulator and devices support different sets of options. Use the information in this type to specify the configuration details for your layer.

## Topics

### Getting the supported formats

var supportedColorFormats: [MTLPixelFormat]

An array of color formats that the layer supports for its textures.

var supportedDepthFormats: [MTLPixelFormat]

The list of depth formats that the layer supports

### Getting the supported layouts

func supportedLayouts(options: LayerRenderer.Capabilities.SupportedLayoutsOptions) -> [LayerRenderer.Layout]

Returns an array of texture layouts that the layer supports.

struct SupportedLayoutsOptions

Options you can use to filter the supported layouts for a layer.

### Getting the supported layer features

var supportsFoveation: Bool

A Boolean value that indicates whether the layer supports variable rasterization rates.

### Getting the minimum near plane distance

var supportedMinimumNearPlaneDistance: Float

The minimum distance in meters to the layer’s near projection plane.

## Relationships

### Conforms To

- Copyable

## See Also

### Configuring the layer renderer

var configuration: LayerRenderer.Configuration

The configuration details for the specified layer.

struct Configuration

A type that stores the texture formats, layout information, and other details you use to configure your rendering loop code.

