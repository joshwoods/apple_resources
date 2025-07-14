

- MetalFX
- MTLFXSpatialScaler
-  inputContentHeight 

Instance Property

# inputContentHeight

The height, in pixels, of the region within the color texture the spatial scaler uses as its input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var inputContentHeight: Int { get set }
```

**Required**

## Discussion

The input content height must be less than or equal to inputHeight.

## See Also

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

