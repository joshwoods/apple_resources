

- Metal
- MTLResourceStateCommandEncoder
-  updateTextureMapping(\_:mode:region:mipLevel:slice:) 

Instance Method

# updateTextureMapping(\_:mode:region:mipLevel:slice:)

Encodes a command to update the texture mappings for a region in a single texture mipmap.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

**Mac Catalyst, macOS**

``` source
optional func updateTextureMapping(
    _ texture: any MTLTexture,
    mode: MTLSparseTextureMappingMode,
    region: MTLRegion,
    mipLevel: Int,
    slice: Int
)
```

**iOS, iPadOS, tvOS, visionOS**

``` source
func updateTextureMapping(
    _ texture: any MTLTexture,
    mode: MTLSparseTextureMappingMode,
    region: MTLRegion,
    mipLevel: Int,
    slice: Int
)
```

**Required**

## Parameters 

`texture`  

The sparse texture to update.

`mode`  

A mode that indicates whether the method allocates or frees a memory tile in the texture.

`region`  

A region, in tile coordinates, that describes the part of the mipmap to update.

`mipLevel`  

The mipmap to update.

`slice`  

The slice in the texture to update.

## Discussion

When the GPU executes the command that updates the texture’s memory mapping, the GPU gets details about the region from the `region` parameter.

To allocate tiles from the heap, pass MTLSparseTextureMappingMode.map as the `mode` parameter, and to free files back to the heap, pass MTLSparseTextureMappingMode.unmap.

If you encode other commands that use the texture’s contents, such as rendering to the texture or sampling from a texture, synchronize the texture’s mapping updates with those commands to avoid race conditions. See Resource Synchronization.

If you encode commands with multiple resource state passes, synchronize the resources to run the commands in the passes sequentially. See the MTLResourceStateCommandEncoder protocol.

## See Also

### Updating Texture Memory Assignments

func updateTextureMappings(any MTLTexture, mode: MTLSparseTextureMappingMode, regions: UnsafePointer&lt;MTLRegion>, mipLevels: UnsafePointer&lt;Int>, slices: UnsafePointer&lt;Int>, numRegions: Int)

Encodes a command to update memory mappings for multiple regions inside a texture.

**Required**

enum MTLSparseTextureMappingMode

Options for sparse texture mapping.

