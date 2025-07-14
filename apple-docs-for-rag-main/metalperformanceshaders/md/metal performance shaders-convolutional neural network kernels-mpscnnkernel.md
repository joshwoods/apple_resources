

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNKernel 

Class

# MPSCNNKernel

Base class for neural network layers.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class MPSCNNKernel : MPSKernel
```

## Overview

An MPSCNNKernel object consumes one MPSImage object and produces one MPSImage object.

The region overwritten in the destination image is described by the clipRectproperty. The top left corner of the region consumed (ignoring adjustments for filter size—for example, convolution filter size) is given by the offset property. The size of the region consumed is a function of the size of the clipRect property and any subsampling caused by pixel strides at work (for example, `strideInPixelsX``/``strideInPixelsY` in the MPSCNNPooling class). Wherever the offset and clipRect properties would cause an `{x,y}` pixel address not in the image to be read, the edgeMode property is used to determine what value to read there.

The `z` or `depth` component of the offset, origin and size properties indexes which images to use.

- If the MPSImage object contains only a single image, then these values should be `offset.z = 0`, `clipRect.origin.z = 0`, and `clipRect.size.depth = 1`.

- If the MPSImage object contains multiple images, then the value of `clipRect.size.depth` determines the number of images to process. Both the source and destination MPSImage objects must have at least this many images. The value of `offset.z` refers to the starting image index of the source. Thus, the value of `offset.z + clipRect.size.depth` must be `destinationFeatureChannelOffset property can be used to control where the kernel will start writing in terms of feature channel dimension. For example, if the destination has 64 channels and thdestinationFeatureChannelOffsete kernel outputs 32 channels, channels 0-31 of the destination will be populated by the kernel (by default). But if you want the kernel to populate channels 32-63 of the destination, you can set the value of destinationFeatureChannelOffset to 32. Suppose you have a source of dimensions `w x h x Ni`, where `N` is the number of channels, which goes through a convolution filter `C0` which produces the output` O0 = w x h x N0` and `C`1 which produces the output `O1 = w x h x N1` followed by concatenation which produces `O = w x h x (N0 + N1)`. You can achieve this by creating an MPSImage object with dimensions `w x h x (N0 + N1)` and using this as the destination of both convolutions as follows:

- `C0: destinationFeatureChannelOffset = 0`, this will output `N0` channels starting at channel `0` of destination thus populating `[0,N0-1]` channels.

- `C1: destinationFeatureChannelOffset = N0`, this will output `N1` channels starting at channel `N0` of destination thus populating `[N0,N0+N1-1]` channels.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Instance Properties

var offset: MPSOffset

The position of the destination image's clip rectangle origin, relative to the source image.

struct MPSOffset

A signed coordinate with x, y, and z components.

var clipRect: MTLRegion

An optional clip rectangle to use when writing data. Only the pixels in the clip rectangle will be overwritten.

struct MTLRegion

The bounds for a subset of an object’s elements.

var destinationFeatureChannelOffset: Int

The number of channels in the destination image to skip before writing output data.

var edgeMode: MPSImageEdgeMode

The edge mode to use when texture reads stray off the edge of an image.

enum MPSImageEdgeMode

The options used to control the edge behavior of an image filter when it reads outside the bounds of a source texture.

var kernelHeight: Int

var kernelWidth: Int

var strideInPixelsX: Int

var strideInPixelsY: Int

var isBackwards: Bool

var padding: any MPSNNPadding

protocol MPSNNPadding

The protocol that provides a description of how kernels should pad images.

var destinationImageAllocator: any MPSImageAllocator

protocol MPSImageAllocator

var dilationRateX: Int

var dilationRateY: Int

var isStateModified: Bool

var sourceFeatureChannelMaxCount: Int

var sourceFeatureChannelOffset: Int

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage) -> MPSImage

func encode(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage, destinationImage: MPSImage)

Encodes a kernel into a command buffer. The ensuing operation proceeds out-of-place.

func appendBatchBarrier() -> Bool

func batchEncodingStorageSize(sourceImage: [MPSImage], sourceStates: [[MPSState]]?, destinationImage: [MPSImage]?) -> Int

func destinationImageDescriptor(sourceImages: [MPSImage], sourceStates: [MPSState]?) -> MPSImageDescriptor

func encode(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage, destinationState: MPSState, destinationImage: MPSImage)

func encode(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage, destinationState: AutoreleasingUnsafeMutablePointer&lt;MPSState?>, destinationStateIsTemporary: Bool) -> MPSImage

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage]) -> [MPSImage]

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage], destinationImages: [MPSImage])

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage], destinationStates: [MPSState]?, destinationImages: [MPSImage])

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage], destinationStates: AutoreleasingUnsafeMutablePointer&lt;NSArray?>, destinationStateIsTemporary: Bool) -> [MPSImage]

func encodingStorageSize(sourceImage: MPSImage, sourceStates: [MPSState]?, destinationImage: MPSImage?) -> Int

func isResultStateReusedAcrossBatch() -> Bool

func resultState(sourceImage: MPSImage, sourceStates: [MPSState]?, destinationImage: MPSImage) -> MPSState?

func resultStateBatch(sourceImage: [MPSImage], sourceStates: [[MPSState]]?, destinationImage: [MPSImage]) -> [MPSState]?

func temporaryResultState(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage, sourceStates: [MPSState]?, destinationImage: MPSImage) -> MPSState?

func temporaryResultStateBatch(commandBuffer: any MTLCommandBuffer, sourceImage: [MPSImage], sourceStates: [[MPSState]]?, destinationImage: [MPSImage]) -> [MPSState]?

## Relationships

### Inherits From

- MPSKernel

## See Also

### Layer Base Classes

class MPSCNNBinaryKernel

A convolution neural network kernel.

class MPSCNNGradientKernel

The base class for gradient layers.

