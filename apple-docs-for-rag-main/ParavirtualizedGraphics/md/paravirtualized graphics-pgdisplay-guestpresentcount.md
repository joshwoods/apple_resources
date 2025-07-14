

- Paravirtualized Graphics
- PGDisplay
-  guestPresentCount 

Instance Property

# guestPresentCount

The number of frame presents that the guest has generated since object creation.

Mac Catalyst 14.0+macOS 11.0+

``` source
var guestPresentCount: Int { get }
```

**Required**

## Discussion

This value can exceed the number of times that the framework invokes the newFrameEventHandler block if the host isn’t encoding frames fast enough to keep up.

## See Also

### Handling Frame Updates

var hostPresentCount: Int

The number of unique frames that the host has encoded since object creation.

**Required**

var minimumTextureUsage: MTLTextureUsage

The Metal texture usage flags necessary for any texture that can be a destination for frame data.

**Required**

func encodeCurrentFrame(to: any MTLCommandBuffer, texture: any MTLTexture, region: MTLRegion) -> Bool

Encodes Metal commands to process the current frame and write it to a texture.

**Required**

