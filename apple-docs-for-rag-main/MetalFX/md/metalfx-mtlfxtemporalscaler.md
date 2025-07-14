

- MetalFX
-  MTLFXTemporalScaler 

Protocol

# MTLFXTemporalScaler

An upscaling effect that generates a higher resolution texture in a render pass by analyzing multiple input textures over time.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
protocol MTLFXTemporalScaler : NSObjectProtocol
```

## Overview

The MetalFX temporal scaler increases the size of your input texture to a larger output texture. You can use the scaler to upscale every frame of your app’s scene or rendering in real time. With a scaler, you can draw more complicated scenes in less time by intentionally rendering to a lower resolution to save time before upscaling.

Create an MTLFXTemporalScaler instance by following these steps:

1.  Create and configure an MTLFXTemporalScalerDescriptor instance.

2.  Call the descriptor’s makeTemporalScaler(device:) method.

Upscale a rendering by following these steps for every render pass:

1.  Set the temporal scaler’s colorTexture property to the input texture.

2.  Set the scaler’s inputContentWidth and inputContentHeight properties.

3.  Set the scaler’s outputTexture property to your destination texture.

4.  Encode the upscale commands to an MTLCommandBuffer by calling the temporal scaler’s encode(commandBuffer:) method.

## Topics

### Configuring the image input

var colorTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s input color texture must set to apply the temporal scaler.

**Required**

var colorTexture: (any MTLTexture)?

An input color texture you set for the temporal scaler that supports the correct color texture usage options.

**Required**

var inputContentWidth: Int

The width, in pixels, of the region within the color texture the temporal scaler uses as its input.

**Required**

var inputContentHeight: Int

The height, in pixels, of the region within the color texture the temporal scaler uses as its input.

**Required**

var jitterOffsetX: Float

The horizontal component of the subpixel sampling coordinate you use to generate the color texture input.

**Required**

var jitterOffsetY: Float

The vertical component of the subpixel sampling coordinate you use to generate the color texture input.

**Required**

var exposureTexture: (any MTLTexture)?

A texture that sets the exposure level for the color texture input.

**Required**

var preExposure: Float

The exposure value that you’ve already applied to your color texture input.

**Required**

### Configuring the depth input

var depthTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s input depth texture must set to apply the temporal scaler.

**Required**

var depthTexture: (any MTLTexture)?

An input depth texture you set for the temporal scaler that supports the correct depth texture usage options.

**Required**

var isDepthReversed: Bool

A Boolean value that indicates whether the depth texture uses zero to represent the farthest distance.

**Required**

### Configuring the motion input

var motionTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s input motion texture must set to apply the temporal scaler.

**Required**

var motionTexture: (any MTLTexture)?

An input motion texture you set for the temporal scaler that supports the correct motion texture usage options.

**Required**

var motionVectorScaleX: Float

The horizontal scale factor the temporal scaler applies to the input motion texture.

**Required**

var motionVectorScaleY: Float

The vertical scale factor the temporal scaler applies to the input motion texture.

**Required**

### Configuring the reactive mask input

var reactiveTextureUsage: MTLTextureUsage

The minimal texture-usage options that your app’s reactive-mask texture input needs to have for the temporal scaler.

**Required**

var reactiveMaskTexture: (any MTLTexture)?

A reactive-mask texture input you set for a temporal scaler that supports the correct usage options.

**Required**

### Configuring the image output

var outputTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s output texture must set to apply the temporal scaler.

**Required**

var outputTexture: (any MTLTexture)?

An output texture that supports the correct depth texture usage options.

**Required**

### Synchronizing untracked resources

var fence: (any MTLFence)?

An optional fence instance that you provide to synchronize your app’s untracked resources.

**Required**

### Encoding a temporal scaling effect

var reset: Bool

A Boolean that indicates whether the temporal scaler discards historical data from previous frames.

**Required**

func encode(commandBuffer: any MTLCommandBuffer)

Adds the temporal scaling command to a render pass’s command buffer.

**Required**

### Inspecting the fixed settings

var inputWidth: Int

The width, in pixels, of the input color texture for the temporal scaler.

**Required**

var inputHeight: Int

The height, in pixels, of the input color texture for the temporal scaler.

**Required**

var inputContentMinScale: Float

The smallest scale factor the temporal scaler uses to generate output textures.

**Required**

var inputContentMaxScale: Float

The largest scale factor the temporal scaler uses to generate output textures.

**Required**

var colorTextureFormat: MTLPixelFormat

The pixel format of the input color texture for the temporal scaler.

**Required**

var depthTextureFormat: MTLPixelFormat

The pixel format of the input depth texture for the temporal scaler.

**Required**

var motionTextureFormat: MTLPixelFormat

The pixel format of the input motion texture for the temporal scaler.

**Required**

var outputWidth: Int

The width, in pixels, of the output color texture for the temporal scaler.

**Required**

var outputHeight: Int

The height, in pixels, of the output color texture for the temporal scaler.

**Required**

var outputTextureFormat: MTLPixelFormat

The pixel format of the output color texture for the temporal scaler.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Temporal scaling

Applying temporal antialiasing and upscaling using MetalFX

Reduce render workloads while increasing image detail with MetalFX.

class MTLFXTemporalScalerDescriptor

A set of properties that configure a temporal scaling effect, and a factory method that creates the effect.

