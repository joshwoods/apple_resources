

- MetalFX
- MTLFXTemporalScaler
-  outputTexture 

Instance Property

# outputTexture

An output texture that supports the correct depth texture usage options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var outputTexture: (any MTLTexture)? { get set }
```

**Required**

## Discussion

The texture you set to this property must meet the following requirements:

- The texture’s storageMode property is MTLStorageMode.private.

- The texture’s usage property uses the colorTextureUsage property’s MTLTextureUsage options as a minimum, and can use additional options.

- The texture’s dimensions is equal to the outputWidth and outputHeight properties.

## See Also

### Configuring the image output

var outputTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s output texture must set to apply the temporal scaler.

**Required**

