

- MetalFX
- MTLFXSpatialScaler
-  colorTextureUsage 

Instance Property

# colorTextureUsage

The minimal texture usage options that your app’s input color texture must set to apply the spatial scaler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var colorTextureUsage: MTLTextureUsage { get }
```

**Required**

## Discussion

The input texture you set to the colorTexture property must use the same set (or a superset) of the MTLTextureUsage options in this property.

## See Also

### Configuring the image input

var colorTexture: (any MTLTexture)?

An input color texture you set for the spatial scaler that supports the correct color texture usage options.

**Required**

var inputContentWidth: Int

The width, in pixels, of the region within the color texture the spatial scaler uses as its input.

**Required**

var inputContentHeight: Int

The height, in pixels, of the region within the color texture the spatial scaler uses as its input.

**Required**

