

- Metal
-  MTLMapIndirectArguments 

Structure

# MTLMapIndirectArguments

The data layout for mapping sparse texture regions when using indirect commands.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLMapIndirectArguments
```

## Topics

### Creating Indirect Mapping Arguments

init()

Returns a default data layout for mapping sparse texture regions.

init(regionOriginX: UInt32, regionOriginY: UInt32, regionOriginZ: UInt32, regionSizeWidth: UInt32, regionSizeHeight: UInt32, regionSizeDepth: UInt32, mipMapLevel: UInt32, sliceId: UInt32)

Returns a new data layout for mapping sparse texture regions.

### Specifying Region Origin

var regionOriginX: UInt32

The x coordinate of the region to change, measured in tile coordinates.

var regionOriginY: UInt32

The y coordinate of the region to change, measured in tile coordinates.

var regionOriginZ: UInt32

The z coordinate of the region to change, measured in tile coordinates.

### Specifying Region Dimensions

var regionSizeWidth: UInt32

The width of the region, measured in tile coordinates.

var regionSizeHeight: UInt32

The height of the region, measured in tile coordinates.

var regionSizeDepth: UInt32

The depth of the region, measured in tile coordinates.

### Specifying Texture Location

var mipMapLevel: UInt32

The mipmap to change.

var sliceId: UInt32

The texture slice to change.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Sparse Textures

Managing Sparse Texture Memory

Take direct control of memory allocation for texture data by using sparse textures.

Creating Sparse Heaps and Sparse Textures

Allocate memory for sparse textures by creating a sparse heap.

Converting Between Pixel Regions and Sparse Tile Regions

Learn how a sparse texture’s contents are organized in memory.

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

