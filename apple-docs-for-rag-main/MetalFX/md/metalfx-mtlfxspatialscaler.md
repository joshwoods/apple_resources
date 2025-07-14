

- MetalFX
-  MTLFXSpatialScaler 

Protocol

# MTLFXSpatialScaler

An upscaling effect that generates a higher resolution texture in a render pass by spatially analyzing an input texture.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLFXSpatialScaler : NSObjectProtocol
```

## Overview

The MetalFX spatial scaler increases the size of your input texture to a larger output texture. You can use the scaler to upscale every frame of your app’s scene or rendering in real time. With a scaler, you can draw more complicated scenes in less time by intentionally rendering to a lower resolution to save time before upscaling.

Create an MTLFXSpatialScaler instance following these steps:

1.  Create and configure an MTLFXSpatialScalerDescriptor instance.

2.  Call the descriptor’s makeSpatialScaler(device:) method.

Upscale a rendering by following these steps for every render pass:

1.  Set the spatial scaler’s colorTexture property to the input texture.

2.  Set the scaler’s inputContentWidth and inputContentHeight properties.

3.  Set the scaler’s outputTexture property to your destination texture.

4.  Encode the upscale commands to an MTLCommandBuffer by calling the spatial scaler’s encode(commandBuffer:) method.

## Topics

### Configuring the image input

var colorTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s input color texture must set to apply the spatial scaler.

**Required**

var colorTexture: (any MTLTexture)?

An input color texture you set for the spatial scaler that supports the correct color texture usage options.

**Required**

var inputContentWidth: Int

The width, in pixels, of the region within the color texture the spatial scaler uses as its input.

**Required**

var inputContentHeight: Int

The height, in pixels, of the region within the color texture the spatial scaler uses as its input.

**Required**

### Configuring the image output

var outputTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s output texture must set to apply the spatial scaler.

**Required**

var outputTexture: (any MTLTexture)?

An output texture that supports the correct depth texture usage options.

**Required**

### Synchronizing untracked resources

var fence: (any MTLFence)?

An optional fence instance that you provide to synchronize your app’s untracked resources.

**Required**

### Encoding a spatial scaler

func encode(commandBuffer: any MTLCommandBuffer)

Adds the spatial scaler to a render pass’s command buffer.

**Required**

### Inspecting the fixed settings

var inputWidth: Int

The width, in pixels, of the input color texture for the spatial scaler.

**Required**

var inputHeight: Int

The height, in pixels, of the input color texture for the spatial scaler.

**Required**

var colorTextureFormat: MTLPixelFormat

The pixel format of the input color texture for the spatial scaler.

**Required**

var colorProcessingMode: MTLFXSpatialScalerColorProcessingMode

Reflects the color processing mode you set in this spatial scaler’s descriptor.

**Required**

var outputWidth: Int

The width, in pixels, of the output color texture for the spatial scaler.

**Required**

var outputHeight: Int

The height, in pixels, of the output color texture for the spatial scaler.

**Required**

var outputTextureFormat: MTLPixelFormat

The pixel format of the output color texture for the spatial scaler.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Spatial scaling

class MTLFXSpatialScalerDescriptor

A set of properties that configure a spatial scaling effect, and a factory method that creates the effect.

enum MTLFXSpatialScalerColorProcessingMode

The color space modes for the input and output textures you use with a spatial scaling effect instance.

