

- Paravirtualized Graphics
- PGDisplay
-  minimumTextureUsage 

Instance Property

# minimumTextureUsage

The Metal texture usage flags necessary for any texture that can be a destination for frame data.

Mac Catalyst 14.0+macOS 11.0+

``` source
var minimumTextureUsage: MTLTextureUsage { get }
```

**Required**

## See Also

### Handling Frame Updates

var guestPresentCount: Int

The number of frame presents that the guest has generated since object creation.

**Required**

var hostPresentCount: Int

The number of unique frames that the host has encoded since object creation.

**Required**

func encodeCurrentFrame(to: any MTLCommandBuffer, texture: any MTLTexture, region: MTLRegion) -> Bool

Encodes Metal commands to process the current frame and write it to a texture.

**Required**

