

- MetalFX
- MTLFXTemporalScalerDescriptor
-  motionTextureFormat 

Instance Property

# motionTextureFormat

The pixel format of the input motion texture for the temporal scaler you create with this descriptor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var motionTextureFormat: MTLPixelFormat { get set }
```

## See Also

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

