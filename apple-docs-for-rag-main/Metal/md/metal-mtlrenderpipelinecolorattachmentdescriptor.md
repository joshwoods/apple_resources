

- Metal
-  MTLRenderPipelineColorAttachmentDescriptor 

Class

# MTLRenderPipelineColorAttachmentDescriptor

A color render target that specifies the color configuration and color operations for a render pipeline.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLRenderPipelineColorAttachmentDescriptor
```

## Overview

A MTLRenderPipelineColorAttachmentDescriptor object defines the configuration of a color attachment associated with a rendering pipeline.

The pixelFormat property must be specified for the rendering pipeline state at the color attachment.

Blend operations determine how a source fragment is combined with a destination value in a color attachment to determine the pixel value to be written. The following properties define whether and how blending is performed:

- The isBlendingEnabled property enables blending. The default value is false.

- The writeMask property identifies which color channels are blended. The default value is all, which allows all color channels to be blended.

- The rgbBlendOperation and alphaBlendOperation properties assign the blend operations for RGB and alpha pixel data. The default value for both properties is MTLBlendOperation.add.

- The sourceRGBBlendFactor, sourceAlphaBlendFactor, destinationRGBBlendFactor, and destinationAlphaBlendFactor properties assign the source and destination blend factors. The default value for sourceRGBBlendFactor and sourceAlphaBlendFactor is MTLBlendFactor.one. The default value for destinationRGBBlendFactor and destinationAlphaBlendFactor is MTLBlendFactor.zero.

## Topics

### Specifying Render Pipeline State

var pixelFormat: MTLPixelFormat

The pixel format of the color attachment’s texture.

var writeMask: MTLColorWriteMask

A bitmask that restricts which color channels are written into the texture.

### Controlling the Blend Operation

var isBlendingEnabled: Bool

A Boolean value that determines whether blending is enabled.

var alphaBlendOperation: MTLBlendOperation

The blend operation assigned for the alpha data.

var rgbBlendOperation: MTLBlendOperation

The blend operation assigned for the RGB data.

### Specifying Blend Factors

var destinationAlphaBlendFactor: MTLBlendFactor

The destination blend factor (DBF) used by the alpha blend operation.

var destinationRGBBlendFactor: MTLBlendFactor

The destination blend factor (DBF) used by the RGB blend operation.

var sourceAlphaBlendFactor: MTLBlendFactor

The source blend factor (SBF) used by the alpha blend operation.

var sourceRGBBlendFactor: MTLBlendFactor

The source blend factor (SBF) used by the RGB blend operation.

### Constants

enum MTLBlendOperation

For every pixel, `MTLBlendOperation` determines how to combine and weight the source fragment values with the destination values. Some blend operations multiply the source values by a source blend factor (SBF), multiply the destination values by a destination blend factor (DBF), and then combine the results using addition or subtraction. Other blend operations use either a minimum or maximum function to determine the result.

enum MTLBlendFactor

The source and destination blend factors are often needed to complete specification of a blend operation. In most cases, the blend factor for both RGB values (*F(rgb)*) and alpha values (*F(a)*) are similar to one another, but in some cases, such as `MTLBlendFactorSourceAlphaSaturated`, the blend factor is slightly different. Four blend factors (`MTLBlendFactorBlendColor`, `MTLBlendFactorOneMinusBlendColor`, `MTLBlendFactorBlendAlpha`, and `MTLBlendFactorOneMinusBlendAlpha`) refer to a constant blend color value that is set by the setBlendColor(red:green:blue:alpha:) method of `MTLRenderCommandEncoder`.

struct MTLColorWriteMask

Values used to specify a mask to permit or restrict writing to color channels of a color value. The values red, green, blue, and alpha select one color channel each, and they can be bitwise combined.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Render Pipeline States

protocol MTLRenderPipelineState

An interface that represents a graphics pipeline configuration for a render pass, which the pass applies to the draw commands you encode.

class MTLRenderPipelineDescriptor

An argument of options you pass to a GPU device to get a render pipeline state.

class MTLRenderPipelineFunctionsDescriptor

A collection of functions for updating a render pipeline.

class MTLMeshRenderPipelineDescriptor

An object that configures new render pipeline state objects for mesh shading.

class MTLPipelineBufferDescriptor

The mutability options for a buffer that a render or compute pipeline uses.

class MTLPipelineBufferDescriptorArray

An array of pipeline buffer descriptors.

class MTLRenderPipelineColorAttachmentDescriptorArray

An array of render pipeline color attachment descriptor objects.

class MTLTileRenderPipelineDescriptor

An object that configures new render pipeline state objects for tile shading.

class MTLTileRenderPipelineColorAttachmentDescriptor

A description of a tile-shading render pipeline’s color render target.

struct MTLPipelineOption

Options that determine how Metal prepares the pipeline.

