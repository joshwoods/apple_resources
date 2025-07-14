

- Metal
- MTLDevice
-  sparseTileSize(with:pixelFormat:sampleCount:) 

Instance Method

# sparseTileSize(with:pixelFormat:sampleCount:)

Returns the dimensions of a sparse tile for a texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func sparseTileSize(
    with textureType: MTLTextureType,
    pixelFormat: MTLPixelFormat,
    sampleCount: Int
) -> MTLSize
```

**Required**

## Parameters 

`textureType`  

An MTLTextureType instance.

`pixelFormat`  

An MTLPixelFormat instance.

`sampleCount`  

The number of samples for each pixel.

## Return Value

A new MTLSize instance.

## Mentioned in 

Converting Between Pixel Regions and Sparse Tile Regions

## Discussion

The size of a sparse tile, in bytes, is the same for all sparse textures on a GPU device object. Because the size of pixels may vary, the actual dimensions of a sparse tile vary based on the texture and the pixel format. Use this method to get the dimensions of the tile for a particular format. Use these dimensions when converting regions from pixel-based units to sparse tile units and vice versa.

## See Also

### Working with Sparse Textures

func sparseTileSize(textureType: MTLTextureType, pixelFormat: MTLPixelFormat, sampleCount: Int, sparsePageSize: MTLSparsePageSize) -> MTLSize

Returns the dimensions of a sparse tile for a texture that has a specific sparse page size.

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

enum MTLSparseTextureRegionAlignmentMode

Options used when converting between a pixel-based region within a texture to a tile-based region.

