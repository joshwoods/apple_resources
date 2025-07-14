

- Paravirtualized Graphics
- PGDisplay
-  hostPresentCount 

Instance Property

# hostPresentCount

The number of unique frames that the host has encoded since object creation.

Mac Catalyst 14.0+macOS 11.0+

``` source
var hostPresentCount: Int { get }
```

**Required**

## Discussion

The value of this property can be smaller than the number of times you’ve called the encodeCurrentFrame(to:texture:region:) method if you encode the same frame multiple times.

## See Also

### Handling Frame Updates

var guestPresentCount: Int

The number of frame presents that the guest has generated since object creation.

**Required**

var minimumTextureUsage: MTLTextureUsage

The Metal texture usage flags necessary for any texture that can be a destination for frame data.

**Required**

func encodeCurrentFrame(to: any MTLCommandBuffer, texture: any MTLTexture, region: MTLRegion) -> Bool

Encodes Metal commands to process the current frame and write it to a texture.

**Required**

