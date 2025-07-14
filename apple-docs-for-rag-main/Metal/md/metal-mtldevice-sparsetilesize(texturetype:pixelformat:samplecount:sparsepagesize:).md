

- Metal
- MTLDevice
-  sparseTileSize(textureType:pixelFormat:sampleCount:sparsePageSize:) 

Instance Method

# sparseTileSize(textureType:pixelFormat:sampleCount:sparsePageSize:)

Returns the dimensions of a sparse tile for a texture that has a specific sparse page size.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func sparseTileSize(
    textureType: MTLTextureType,
    pixelFormat: MTLPixelFormat,
    sampleCount: Int,
    sparsePageSize: MTLSparsePageSize
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

`sparsePageSize`  

An MTLSparsePageSize instance.

## Return Value

A new MTLSize instance.

## See Also

### Working with Sparse Textures

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

enum MTLSparseTextureRegionAlignmentMode

Options used when converting between a pixel-based region within a texture to a tile-based region.

