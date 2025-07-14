

- MetalFX
- MTLFXSpatialScaler
-  outputWidth 

Instance Property

# outputWidth

The width, in pixels, of the output color texture for the spatial scaler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var outputWidth: Int { get }
```

**Required**

## See Also

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

var outputHeight: Int

The height, in pixels, of the output color texture for the spatial scaler.

**Required**

var outputTextureFormat: MTLPixelFormat

The pixel format of the output color texture for the spatial scaler.

**Required**

