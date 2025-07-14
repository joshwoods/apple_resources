

- Metal
-  MTLTexture 

Protocol

# MTLTexture

A resource that holds formatted image data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLTexture : MTLResource
```

## Mentioned in 

Setting Resource Storage Modes

Improving CPU Performance by Using Argument Buffers

Synchronizing a Managed Resource in macOS

Creating a Mipmapped Texture

Simplifying GPU Resource Management with Residency Sets

## Overview

Don’t implement this protocol yourself; instead, use one of the following methods to create a MTLTexture instance:

- Create an MTLTextureDescriptor instance to describe the texture’s properties and then call the makeTexture(descriptor:) method of the MTLDevice protocol to create the texture.

- To create a texture that uses an existing IOSurface to hold the texture data, create an MTLTextureDescriptor instance to describe the image data in the surface. Call the makeTexture(descriptor:iosurface:plane:) method to create the texture.

- To create a texture that reinterprets another texture’s data as if it has a different format, call one of the following texture methods:

  - makeTextureView(pixelFormat:)

  - makeTextureView(pixelFormat:textureType:levels:slices:) (Swift)

  - newTextureViewWithPixelFormat:textureType:levels:slices: (Objective-C)

  You need to choose a pixel format for the new texture compatible with the source texture’s pixel format. The new texture shares the same storage allocation as the source texture. If you make changes to the new texture, the source texture reflects those changes, and vice versa.

- To create a texture that uses an MTLBuffer instance’s contents to hold pixel data, create an MTLTextureDescriptor object to describe the texture’s properties. Then call the makeTexture(descriptor:offset:bytesPerRow:) method on the buffer object. The new texture object shares the storage allocation of the source buffer object. If you make changes to the texture, the buffer reflects those changes, and vice versa.

After you create a MTLTexture object, most of its characteristics, such as its size, type, and pixel format are all immutable. Only the texture’s pixel data is mutable.

To copy pixel data from system memory into the texture, call replace(region:mipmapLevel:slice:withBytes:bytesPerRow:bytesPerImage:) or replace(region:mipmapLevel:withBytes:bytesPerRow:).

To copy pixel data back to system memory, call getBytes(_:bytesPerRow:bytesPerImage:from:mipmapLevel:slice:) or getBytes(_:bytesPerRow:from:mipmapLevel:).

## Topics

### Copying Data into a Texture Image

func replace(region: MTLRegion, mipmapLevel: Int, slice: Int, withBytes: UnsafeRawPointer, bytesPerRow: Int, bytesPerImage: Int)

Copies pixel data into a section of a texture slice.

**Required**

func replace(region: MTLRegion, mipmapLevel: Int, withBytes: UnsafeRawPointer, bytesPerRow: Int)

Copies a block of pixels into a section of texture slice 0.

**Required**

### Copying Data from a Texture Image

func getBytes(UnsafeMutableRawPointer, bytesPerRow: Int, bytesPerImage: Int, from: MTLRegion, mipmapLevel: Int, slice: Int)

Copies pixel data from the texture to a buffer in system memory.

**Required**

func getBytes(UnsafeMutableRawPointer, bytesPerRow: Int, from: MTLRegion, mipmapLevel: Int)

Copies pixel data from the first slice of the texture to a buffer in system memory.

**Required**

### Creating Textures by Reinterpreting Existing Texture Data

func makeTextureView(pixelFormat: MTLPixelFormat) -> (any MTLTexture)?

Creates a new view of the texture, reinterpreting its data using a different pixel format.

**Required**

func makeTextureView(pixelFormat: MTLPixelFormat, textureType: MTLTextureType, levels: Range&lt;Int>, slices: Range&lt;Int>) -> (any MTLTexture)?

Creates a new view of the texture, reinterpreting a subset of its data using a different type and pixel format.

func makeTextureView(pixelFormat: MTLPixelFormat, textureType: MTLTextureType, levels: Range&lt;Int>, slices: Range&lt;Int>, swizzle: MTLTextureSwizzleChannels) -> (any MTLTexture)?

Creates a new view of the texture, reinterpreting a subset of its data using a different type, pixel format, and swizzle pattern.

### Querying Texture Attributes

var textureType: MTLTextureType

The dimension and arrangement of the texture image data.

**Required**

var pixelFormat: MTLPixelFormat

The format of pixels in the texture.

**Required**

var width: Int

The width of the texture image for the base level mipmap, in pixels.

**Required**

var height: Int

The height of the texture image for the base level mipmap, in pixels.

**Required**

var depth: Int

The depth of the texture image for the base level mipmap, in pixels.

**Required**

var mipmapLevelCount: Int

The number of mipmap levels in the texture.

**Required**

var arrayLength: Int

The number of slices in the texture array.

**Required**

var sampleCount: Int

The number of samples in each pixel.

**Required**

var isFramebufferOnly: Bool

A Boolean value that indicates whether the texture can only be used as a render target.

**Required**

var usage: MTLTextureUsage

Options that determine how you can use the texture.

**Required**

var allowGPUOptimizedContents: Bool

A Boolean value indicating whether the GPU is allowed to adjust the contents of the texture to improve GPU performance.

**Required**

var isShareable: Bool

A Boolean indicating whether this texture can be shared with other processes.

**Required**

var swizzle: MTLTextureSwizzleChannels

The pattern that the GPU applies to pixels when you read or sample pixels from the texture.

**Required**

enum MTLTextureType

The dimension of each image, including whether multiple images are arranged into an array or a cube.

struct MTLTextureUsage

An enumeration for the various options that determine how you can use a texture.

### Getting Information about the IOSurface the Texture Was Created From

var iosurface: IOSurfaceRef?

A reference to the underlying surface instance for the texture, if applicable.

**Required**

var iosurfacePlane: Int

The number of a plane within the underlying surface instance for the texture, if applicable.

**Required**

### Getting Information about Ancestor Resources

var parent: (any MTLTexture)?

The parent texture used to create this texture, if any.

**Required**

var parentRelativeLevel: Int

The base level of the parent texture used to create this texture.

**Required**

var parentRelativeSlice: Int

The base slice of the parent texture used to create this texture.

**Required**

var buffer: (any MTLBuffer)?

The source buffer used to create this texture, if any.

**Required**

var bufferOffset: Int

The offset in the source buffer where the texture’s data comes from.

**Required**

var bufferBytesPerRow: Int

The number of bytes in each row of the texture’s source buffer.

**Required**

var rootResource: (any MTLResource)?

The resource that owns the storage for this texture.

**Required**

Deprecated

### Creating a Shared Texture Handle

func makeSharedTextureHandle() -> MTLSharedTextureHandle?

Creates a new texture handle from a shareable texture.

**Required**

### Creating Views of Textures on Other GPUs

func makeRemoteTextureView(any MTLDevice) -> (any MTLTexture)?

Creates a remote texture view for another GPU in the same peer group.

**Required**

var remoteStorageTexture: (any MTLTexture)?

The texture on another GPU that the texture was created from, if any.

**Required**

### Querying Sparse Properties

var isSparse: Bool

A Boolean value that indicates whether this is a sparse texture.

**Required**

var firstMipmapInTail: Int

The index of the first mipmap in the tail.

**Required**

var tailSizeInBytes: Int

The size of the sparse texture tail, in bytes.

**Required**

### Instance Properties

var compressionType: MTLTextureCompressionType

**Required**

var gpuResourceID: MTLResourceID

**Required**

## Relationships

### Inherits From

- MTLAllocation
- MTLResource
- NSObjectProtocol

## See Also

### Texture Basics

Understanding Color-Renderable Pixel Format Sizes

Know the size limits of color render targets in Apple GPUs based on the target’s pixel format.

Optimizing Texture Data

Optimize a texture’s data to improve GPU or CPU access.

enum MTLTextureCompressionType

class MTLTextureDescriptor

An object that you use to configure new Metal texture objects.

class MTKTextureLoader

An object that creates textures from existing data in common image formats.

class MTLSharedTextureHandle

A texture handle that can be shared across process address space boundaries.

enum MTLPixelFormat

The data formats that describe the organization and characteristics of individual pixels in a texture.

