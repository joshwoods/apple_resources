

- MetalFX
- MTLFXTemporalScaler
-  reactiveTextureUsage 

Instance Property

# reactiveTextureUsage

The minimal texture-usage options that your app’s reactive-mask texture input needs to have for the temporal scaler.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+

``` source
var reactiveTextureUsage: MTLTextureUsage { get }
```

**Required**

## Discussion

The input texture you set to the reactiveMaskTexture property needs to use the same set as, or a superset of, the MTLTextureUsage options of this property.

## See Also

### Configuring the reactive mask input

var reactiveMaskTexture: (any MTLTexture)?

A reactive-mask texture input you set for a temporal scaler that supports the correct usage options.

**Required**

