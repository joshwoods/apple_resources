

- Metal
-  MTLResourceStateCommandEncoder 

Protocol

# MTLResourceStateCommandEncoder

An encoder that encodes commands that modify resource configurations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLResourceStateCommandEncoder : MTLCommandEncoder
```

## Mentioned in 

Assigning Memory to Sparse Textures

## Overview

Use a resource state command encoder to manage memory mappings for sparse textures.

Your app does not define classes that implement this protocol. To create a MTLResourceStateCommandEncoder object, call the makeResourceStateCommandEncoder() method of the MTLCommandBuffer object into which you want to encode blit commands. Next, call methods on the MTLResourceStateCommandEncoder object to enqueue state updates. Finally, call endEncoding() to finish the encoding process.

## Topics

### Updating Texture Memory Assignments

func updateTextureMapping(any MTLTexture, mode: MTLSparseTextureMappingMode, region: MTLRegion, mipLevel: Int, slice: Int)

Encodes a command to update the texture mappings for a region in a single texture mipmap.

**Required**

func updateTextureMappings(any MTLTexture, mode: MTLSparseTextureMappingMode, regions: UnsafePointer&lt;MTLRegion>, mipLevels: UnsafePointer&lt;Int>, slices: UnsafePointer&lt;Int>, numRegions: Int)

Encodes a command to update memory mappings for multiple regions inside a texture.

**Required**

enum MTLSparseTextureMappingMode

Options for sparse texture mapping.

### Updating Texture Memory Assignments Indirectly

func updateTextureMapping(any MTLTexture, mode: MTLSparseTextureMappingMode, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes a command to update a texture’s memory mappings, specifying the parameters indirectly.

**Required**

### Performing Fence Operations

func update(any MTLFence)

Encodes a command that instructs the GPU to update a fence, which signals passes waiting on the fence.

**Required**

func wait(for: any MTLFence)

Encodes a command that instructs the GPU to pause before starting the resource state commands until another pass updates a fence.

**Required**

### Instance Methods

func moveTextureMappings(sourceTexture: any MTLTexture, sourceSlice: Int, sourceLevel: Int, sourceOrigin: MTLOrigin, sourceSize: MTLSize, destinationTexture: any MTLTexture, destinationSlice: Int, destinationLevel: Int, destinationOrigin: MTLOrigin)

**Required**

## Relationships

### Inherits From

- MTLCommandEncoder
- NSObjectProtocol

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

struct MTLMapIndirectArguments

The data layout for mapping sparse texture regions when using indirect commands.

