

- Metal
- Textures
-  Converting Between Pixel Regions and Sparse Tile Regions 

Article

# Converting Between Pixel Regions and Sparse Tile Regions

Learn how a sparse texture’s contents are organized in memory.

## Overview

In Metal, when you create textures or copy data into or out of them, you specify sizes and regions in pixels. (Usually, this means creating MTLSize and MTLRegion structures that specify sizes and offsets in pixel units.) You still use MTLSize and MTLRegion when working with sparse textures. However, some new actions, such as mapping and unmapping of memory in sparse textures, require you to specify sizes in tile-sized units instead. Metal provides utility methods that convert between pixel measurements and tile-sized measurements.

### Determine the Dimensions of a Sparse Tile

All sparse tiles created by a given device object have the same size in bytes. However, the number of pixels in a sparse tile varies for each texture, depending on pixel size. To get the dimensions, in pixels, of a sparse tile for a specific texture format, call the sparseTileSize(with:pixelFormat:sampleCount:) method on the device object, passing in the texture format and sample count:

```
MTLSize tileSize = [_device sparseTileSizeWithTextureType:MTLTextureType2D
                        pixelFormat:MTLPixelFormatBGRA8Unorm
                        sampleCount:1];
```

All tiles in a texture have the same dimensions, and the texture is laid out as a grid of sparse tiles. For example, the following texture image is `256 x 256` pixels.

If the tile size is `64 x 64`, to cover the texture, you need a `4 x 4` grid of sparse tiles. A MTLRegion in tile coordinates with an origin of `(0,0)` and a size of `(1,1)` corresponds to a pixel region with an origin of `(0,0)` and a size of `(64,64)`. Similarly, a tile region with an origin of `(2,1)` and a size of `(2,3)` corresponds to a pixel region with an origin of `(128,64)` and a size of `(128,196)`.

### Convert from Pixels to Tiles

To convert from a pixel region to a tile region, call the convertSparsePixelRegions(_:toTileRegions:withTileSize:alignmentMode:numRegions:) method on a device object, as shown in the code below:

```
MTLRegion pixelRegion[1] = { MTLRegionMake2D(64, 64, 128, 128)};
MTLRegion tileRegion[1];

[_device convertSparsePixelRegions:pixelRegion
                     toTileRegions:tileRegion
                      withTileSize:tileSize
                     alignmentMode:MTLSparseTextureRegionAlignmentModeOutward
                        numRegions:1];
```

If the pixel region doesn’t precisely align to the tile size, the alignment mode parameter determines whether the tile region expands outward to encompass any partially covered tiles (MTLSparseTextureRegionAlignmentMode.outward) or whether those partially covered regions are ignored (MTLSparseTextureRegionAlignmentMode.inward).

### Convert from Tiles to Pixels

Similarly, you can convert from tile units into pixel units. The resulting pixel region is always aligned to tile boundaries, so you don’t need to specify an alignment parameter.

```
[_device convertSparseTileRegions:&tileRegion
                   toPixelRegions:&pixelRegion
                     withTileSize:tileSize
                       numRegions:1];
```

## See Also

### Sparse Textures

Managing Sparse Texture Memory

Take direct control of memory allocation for texture data by using sparse textures.

Creating Sparse Heaps and Sparse Textures

Allocate memory for sparse textures by creating a sparse heap.

Assigning Memory to Sparse Textures

Use a resource state encoder to allocate and deallocate sparse tiles for a sparse texture.

Reading and Writing to Sparse Textures

Decide how to handle access to unmapped texture regions.

Estimating How Often a Texture Region Is Accessed

Use texture access patterns to determine when you need to map a texture region.

class MTLResourceStatePassDescriptor

A configuration for a resource state pass, used to create a resource state command encoder.

class MTLResourceStatePassSampleBufferAttachmentDescriptor

A description of where to store GPU counter information at the start and end of a resource state pass.

class MTLResourceStatePassSampleBufferAttachmentDescriptorArray

An array of sample buffer attachments for a resource state pass.

protocol MTLResourceStateCommandEncoder

An encoder that encodes commands that modify resource configurations.

struct MTLMapIndirectArguments

The data layout for mapping sparse texture regions when using indirect commands.

