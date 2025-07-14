

- MetalFX
- MTLFXTemporalScaler
-  depthTextureFormat 

Instance Property

# depthTextureFormat

The pixel format of the input depth texture for the temporal scaler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var depthTextureFormat: MTLPixelFormat { get }
```

**Required**

## See Also

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

