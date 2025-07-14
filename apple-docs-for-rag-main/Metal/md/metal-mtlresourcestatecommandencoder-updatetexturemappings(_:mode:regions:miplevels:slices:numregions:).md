

- Metal
- MTLResourceStateCommandEncoder
-  updateTextureMappings(\_:mode:regions:mipLevels:slices:numRegions:) 

Instance Method

# updateTextureMappings(\_:mode:regions:mipLevels:slices:numRegions:)

Encodes a command to update memory mappings for multiple regions inside a texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

**iOS, iPadOS, tvOS, visionOS**

``` source
func updateTextureMappings(
    _ texture: any MTLTexture,
    mode: MTLSparseTextureMappingMode,
    regions: UnsafePointer,
    mipLevels: UnsafePointer,
    slices: UnsafePointer,
    numRegions: Int
)
```

**Mac Catalyst, macOS**

``` source
optional func updateTextureMappings(
    _ texture: any MTLTexture,
    mode: MTLSparseTextureMappingMode,
    regions: UnsafePointer,
    mipLevels: UnsafePointer,
    slices: UnsafePointer,
    numRegions: Int
)
```

**Required**

## Parameters 

`texture`  

The sparse texture to update.

`mode`  

The change to make to the texture mapping.

`regions`  

A pointer to an array of regions to change. You must provide as many regions as you specify in the `numRegions` parameter.

`mipLevels`  

A pointer to an array of mipmap levels to change. You must provide as many entries as you specify in the `numRegions` parameter.

`slices`  

A pointer to an array of slices to change. You must provide as many entries as you specify in the `numRegions` parameter.

`numRegions`  

The number of regions to update.

## See Also

### Updating Texture Memory Assignments

func updateTextureMapping(any MTLTexture, mode: MTLSparseTextureMappingMode, region: MTLRegion, mipLevel: Int, slice: Int)

Encodes a command to update the texture mappings for a region in a single texture mipmap.

**Required**

enum MTLSparseTextureMappingMode

Options for sparse texture mapping.

