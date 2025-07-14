

- MetalFX
-  MTLFXSpatialScalerDescriptor 

Class

# MTLFXSpatialScalerDescriptor

A set of properties that configure a spatial scaling effect, and a factory method that creates the effect.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLFXSpatialScalerDescriptor
```

## Topics

### Checking a GPU device’s scaling support

class func supportsDevice(any MTLDevice) -> Bool

Returns a Boolean value that indicates whether the spatial scaler works with a GPU.

### Configuring a spatial scaler’s input

var inputWidth: Int

The width of the input color texture for the spatial scaler you create with this descriptor.

var inputHeight: Int

The height of the input color texture for the spatial scaler you create with this descriptor.

var colorTextureFormat: MTLPixelFormat

The pixel format of the input color texture for the spatial scaler you create with this descriptor.

var colorProcessingMode: MTLFXSpatialScalerColorProcessingMode

The color space of the input color texture for the spatial scaler you create with this descriptor.

### Configuring a spatial scaler’s output

var outputWidth: Int

The width of the output color texture for the spatial scaler you create with this descriptor.

var outputHeight: Int

The height of the output color texture for the spatial scaler you create with this descriptor.

var outputTextureFormat: MTLPixelFormat

The pixel format of the output color texture for the spatial scaler you create with this descriptor.

### Creating spatial scaler instances

func makeSpatialScaler(device: any MTLDevice) -> (any MTLFXSpatialScaler)?

Creates a spatial scaler instance from this descriptor’s current property values.

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

### Spatial scaling

protocol MTLFXSpatialScaler

An upscaling effect that generates a higher resolution texture in a render pass by spatially analyzing an input texture.

enum MTLFXSpatialScalerColorProcessingMode

The color space modes for the input and output textures you use with a spatial scaling effect instance.

