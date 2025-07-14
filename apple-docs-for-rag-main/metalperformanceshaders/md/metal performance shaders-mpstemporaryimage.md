

- Metal Performance Shaders
-  MPSTemporaryImage 

Class

# MPSTemporaryImage

A texture for use in convolutional neural networks that stores transient data to be used and discarded promptly.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class MPSTemporaryImage : MPSImage
```

## Overview

`MPSTemporaryImage` objects can provide a profound reduction in the aggregate texture memory and associated CPU-side allocation cost in your app. Metal Performance Shaders achieves this by automatically identifying `MPSTemporaryImage` objects that do not overlap in time over the course of a MTLCommandBuffer object’s lifetime and can therefore reuse the same memory. `MPSTemporaryImage` objects leverage an internal cache of preallocated reusable memory to hold pixel data to avoid typical memory allocation performance penalties common to ordinary MPSImage and MTLTexture objects.

To avoid data corruption due to aliasing, `MPSTemporaryImage` objects impose some important restrictions:

- The underlying texture storage mode is MTLStorageMode.private. You cannot, for example, use the getBytes(_:bytesPerRow:from:mipmapLevel:) or replace(region:mipmapLevel:withBytes:bytesPerRow:) methods with them. Temporary images are strictly read and written by the GPU.

- The temporary image may be used only on a single MTLCommandBuffer object. This limits the chronology to a single linear time stream.

- The readCount property must be managed correctly.

- Temporary images must also adhere to the general pixel format restrictions for MPSImage objects.

Since temporary images can only be used with a single command buffer, and can not be used off the GPU, they generally should not be kept around past the completion of their associated command buffer. The lifetime of a temporary image is typically expected to be extremely short, perhaps spanning only a few lines of code.

To keep the lifetime of the underlying texture allocation as short as possible, the texture is not allocated until the first time the `MPSTemporaryImage` object is used by an MPSCNNKernel object or until the first time the texture property is read. The readCount property serves to limit the lifetime of the texture on deallocation.

You may use the texture property with the `encode` methods of an MPSUnaryImageKernel subclass, if `featureChannelsreadCount property is not modified, since the enclosing object is not available. There is no locking mechanism provided to prevent a MTLTexture object returned from the texture property from becoming invalid when the value of the readCount property reaches 0.

`MPSTemporaryImage` objects can otherwise be used wherever MPSImage objects are used.

### The MPSTemporaryImage Class

The MPSTemporaryImage class extends the MPSImage class to provide advanced caching of unused memory, in order to increase performance and reduce memory footprint. MPSTemporaryImage objects are intended as fast GPU-only storage for intermediate image data needed only transiently within a single MTLCommandBuffer object. They accelerate the common case of image data which is created only to be consumed and destroyed immediately by the next operation(s) encoded in a command buffer. MPSTemporaryImage objects provide a convenient and simple way to save memory by automatically aliasing other MPSTemporaryImage objects in the same command buffer. Because they alias (i.e., share texel storage with) other textures in the same command buffer, the valid lifetime of the data in an MPSTemporaryImage object is extremely short, limited to a portion of a the command buffer itself.

You can not read or write data to an MPSTemporaryImage using the CPU, or use the data in other MTLCommandBuffer objects. Use regular MPSImage objects for more persistent storage.

## Topics

### Initializers

init(commandBuffer: any MTLCommandBuffer, imageDescriptor: MPSImageDescriptor)

Initializes a temporary image for use on a command buffer.

class MPSImageDescriptor

A description of the attributes used to create an MPSImage.

init(commandBuffer: any MTLCommandBuffer, textureDescriptor: MTLTextureDescriptor)

Low-level interface for creating a temporary image using a texture descriptor.

class MTLTextureDescriptor

An object that you use to configure new Metal texture objects.

init(commandBuffer: any MTLCommandBuffer, textureDescriptor: MTLTextureDescriptor, featureChannels: Int)

### Methods

class func prefetchStorage(with: any MTLCommandBuffer, imageDescriptorList: [MPSImageDescriptor])

A method that helps the framework decide which allocations to make ahead of time.

### Methods to Get an Image Allocator

class func defaultAllocator() -> any MPSImageAllocator

protocol MPSImageAllocator

### Properties

var readCount: Int

The number of times a temporary image may be read by a CNN kernel before its contents become undefined.

## Relationships

### Inherits From

- MPSImage

## See Also

### Neural Networks

Training a Neural Network with Metal Performance Shaders

Use an MPS neural network graph to train a simple neural network digit classifier.

class MPSImage

A texture that may have more than four channels for use in convolutional neural networks.

Objects that Simplify the Creation of Neural Networks

Simplify the creation of neural networks using networks of filter, image, and state nodes.

Convolutional Neural Network Kernels

Build neural networks with layers.

Recurrent Neural Networks

Create recurrent neural networks.

