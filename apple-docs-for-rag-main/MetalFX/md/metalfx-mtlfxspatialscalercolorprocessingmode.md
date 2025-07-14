

- MetalFX
-  MTLFXSpatialScalerColorProcessingMode 

Enumeration

# MTLFXSpatialScalerColorProcessingMode

The color space modes for the input and output textures you use with a spatial scaling effect instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum MTLFXSpatialScalerColorProcessingMode
```

## Topics

### Color space modes

case linear

Indicates your input and output textures use a linear color space.

case perceptual

Indicates your input and output textures use a perceptual color space.

case hdr

Indicates your input and output textures use a high dynamic range color space.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Spatial scaling

protocol MTLFXSpatialScaler

An upscaling effect that generates a higher resolution texture in a render pass by spatially analyzing an input texture.

class MTLFXSpatialScalerDescriptor

A set of properties that configure a spatial scaling effect, and a factory method that creates the effect.

