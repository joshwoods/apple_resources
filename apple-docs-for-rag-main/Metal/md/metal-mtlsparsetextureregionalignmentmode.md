

- Metal
-  MTLSparseTextureRegionAlignmentMode 

Enumeration

# MTLSparseTextureRegionAlignmentMode

Options used when converting between a pixel-based region within a texture to a tile-based region.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
enum MTLSparseTextureRegionAlignmentMode
```

## Topics

### Specifying the Alignment Mode

case outward

The tile region includes any partially covered tiles.

case inward

The tile region ignores partially covered tiles.

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

### Working with Sparse Textures

func sparseTileSize(textureType: MTLTextureType, pixelFormat: MTLPixelFormat, sampleCount: Int, sparsePageSize: MTLSparsePageSize) -> MTLSize

Returns the dimensions of a sparse tile for a texture that has a specific sparse page size.

**Required**

func sparseTileSize(with: MTLTextureType, pixelFormat: MTLPixelFormat, sampleCount: Int) -> MTLSize

Returns the dimensions of a sparse tile for a texture.

**Required**

func sparseTileSizeInBytes(sparsePageSize: MTLSparsePageSize) -> Int

Returns the size, in bytes, of a sparse tile the GPU device creates with a specific page size.

**Required**

var sparseTileSizeInBytes: Int

Returns the size, in bytes, of a sparse tile the GPU device creates using a default page size.

**Required**

func convertSparsePixelRegions(UnsafePointer&lt;MTLRegion>, toTileRegions: UnsafeMutablePointer&lt;MTLRegion>, withTileSize: MTLSize, alignmentMode: MTLSparseTextureRegionAlignmentMode, numRegions: Int)

Converts a list of sparse pixel regions to tile regions.

func convertSparseTileRegions(UnsafePointer&lt;MTLRegion>, toPixelRegions: UnsafeMutablePointer&lt;MTLRegion>, withTileSize: MTLSize, numRegions: Int)

Converts a list of sparse tile regions to pixel regions.

enum MTLSparsePageSize

The page size options, in kilobytes, for sparse textures.

