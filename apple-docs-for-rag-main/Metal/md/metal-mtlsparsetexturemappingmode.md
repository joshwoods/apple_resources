

- Metal
-  MTLSparseTextureMappingMode 

Enumeration

# MTLSparseTextureMappingMode

Options for sparse texture mapping.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
enum MTLSparseTextureMappingMode
```

## Topics

### Specifying the Mapping Mode

case map

A request to map sparse tiles from the heap to a region in the texture.

case unmap

A request to remove any mappings for a region in the texture.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Updating Texture Memory Assignments

func updateTextureMapping(any MTLTexture, mode: MTLSparseTextureMappingMode, region: MTLRegion, mipLevel: Int, slice: Int)

Encodes a command to update the texture mappings for a region in a single texture mipmap.

**Required**

func updateTextureMappings(any MTLTexture, mode: MTLSparseTextureMappingMode, regions: UnsafePointer&lt;MTLRegion>, mipLevels: UnsafePointer&lt;Int>, slices: UnsafePointer&lt;Int>, numRegions: Int)

Encodes a command to update memory mappings for multiple regions inside a texture.

**Required**

