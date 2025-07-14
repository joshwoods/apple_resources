

- Metal
- MTLBlitCommandEncoder
-  resetTextureAccessCounters(\_:region:mipLevel:slice:) 

Instance Method

# resetTextureAccessCounters(\_:region:mipLevel:slice:)

Encodes a command that resets a sparse texture’s access data for a specific region, mipmap level, and slice.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

**iOS, iPadOS, tvOS, visionOS**

``` source
func resetTextureAccessCounters(
    _ texture: any MTLTexture,
    region: MTLRegion,
    mipLevel: Int,
    slice: Int
)
```

**Mac Catalyst, macOS**

``` source
optional func resetTextureAccessCounters(
    _ texture: any MTLTexture,
    region: MTLRegion,
    mipLevel: Int,
    slice: Int
)
```

**Required**

## Parameters 

`texture`  

A sparse texture instance.

`region`  

A region within the sparse texture’s `mipLevel`, in sparse tile coordinates.

`mipLevel`  

A mipmap level within the sparse texture.

`slice`  

A slice within the sparse texture.

## See Also

### Working with Sparse Texture Access Counters

func getTextureAccessCounters(any MTLTexture, region: MTLRegion, mipLevel: Int, slice: Int, resetCounters: Bool, countersBuffer: any MTLBuffer, countersBufferOffset: Int)

Encodes a command that retrieves a sparse texture’s access data for a specific region, mipmap level, and slice.

**Required**

