

- MetalFX
-  MTLFXTemporalScalerDescriptor 

Class

# MTLFXTemporalScalerDescriptor

A set of properties that configure a temporal scaling effect, and a factory method that creates the effect.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
class MTLFXTemporalScalerDescriptor
```

## Topics

### Checking a GPU device’s scaling support

class func supportsDevice(any MTLDevice) -> Bool

Returns a Boolean value that indicates whether the temporal scaler works with a GPU.

class func supportedInputContentMinScale(device: any MTLDevice) -> Float

Returns the smallest temporal scaling factor the device supports as a floating-point value.

class func supportedInputContentMaxScale(device: any MTLDevice) -> Float

Returns the largest temporal scaling factor the device supports as a floating-point value.

### Configuring a temporal effect’s input

var inputWidth: Int

The width of the input color texture for the temporal scaler you create with this descriptor.

var inputHeight: Int

The height of the input color texture for the temporal scaler you create with this descriptor.

var isInputContentPropertiesEnabled: Bool

A Boolean value that indicates whether the temporal scaler you create with this descriptor uses dynamic resolution.

var inputContentMinScale: Float

The smallest scale factor the temporal scaler you create with this descriptor can use to generate output textures.

var inputContentMaxScale: Float

The largest scale factor the temporal scaler you create with this descriptor can use to generate output textures.

var colorTextureFormat: MTLPixelFormat

The pixel format of the input color texture for the temporal scaler you create with this descriptor.

var motionTextureFormat: MTLPixelFormat

The pixel format of the input motion texture for the temporal scaler you create with this descriptor.

var depthTextureFormat: MTLPixelFormat

The pixel format of the input depth texture for the temporal scaler you create with this descriptor.

var isAutoExposureEnabled: Bool

A Boolean value that indicates whether MetalFX calculates the exposure for each frame.

var requiresSynchronousInitialization: Bool

A Boolean value that indicates whether MetalFX compiles a temporal scaling effect’s underlying upscaler as it creates the instance.

var isReactiveMaskTextureEnabled: Bool

A Boolean value that indicates whether a temporal scaler you create with the descriptor applies a reactive mask.

var reactiveMaskTextureFormat: MTLPixelFormat

The pixel format of the reactive mask input texture for a temporal scaler you create with the descriptor.

### Configuring a temporal effect’s output

var outputWidth: Int

The width of the output color texture for the temporal scaler you create with this descriptor.

var outputHeight: Int

The height of the output color texture for the temporal scaler you create with this descriptor.

var outputTextureFormat: MTLPixelFormat

The pixel format of the output color texture for the temporal scaler you create with this descriptor.

### Creating temporal scaling effect instances

func makeTemporalScaler(device: any MTLDevice) -> (any MTLFXTemporalScaler)?

Creates a temporal scaler instance from this descriptor’s current property values.

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

### Temporal scaling

Applying temporal antialiasing and upscaling using MetalFX

Reduce render workloads while increasing image detail with MetalFX.

protocol MTLFXTemporalScaler

An upscaling effect that generates a higher resolution texture in a render pass by analyzing multiple input textures over time.

