

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNBinaryKernel 

Class

# MPSCNNBinaryKernel

A convolution neural network kernel.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSCNNBinaryKernel : MPSKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Instance Properties

var clipRect: MTLRegion

var destinationFeatureChannelOffset: Int

var destinationImageAllocator: any MPSImageAllocator

var isBackwards: Bool

var padding: any MPSNNPadding

var primaryEdgeMode: MPSImageEdgeMode

var primaryOffset: MPSOffset

var primaryStrideInPixelsX: Int

var primaryStrideInPixelsY: Int

var secondaryEdgeMode: MPSImageEdgeMode

var secondaryOffset: MPSOffset

var secondaryStrideInPixelsX: Int

var secondaryStrideInPixelsY: Int

var isStateModified: Bool

var primaryDilationRateX: Int

var primaryDilationRateY: Int

var primaryKernelHeight: Int

var primaryKernelWidth: Int

var primarySourceFeatureChannelMaxCount: Int

var primarySourceFeatureChannelOffset: Int

var secondaryDilationRateX: Int

var secondaryDilationRateY: Int

var secondaryKernelHeight: Int

var secondaryKernelWidth: Int

var secondarySourceFeatureChannelMaxCount: Int

var secondarySourceFeatureChannelOffset: Int

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, primaryImage: MPSImage, secondaryImage: MPSImage) -> MPSImage

func encode(commandBuffer: any MTLCommandBuffer, primaryImage: MPSImage, secondaryImage: MPSImage, destinationImage: MPSImage)

func appendBatchBarrier() -> Bool

func batchEncodingStorageSize(primaryImage: [MPSImage], secondaryImage: [MPSImage], sourceStates: [[MPSState]]?, destinationImage: [MPSImage]?) -> Int

func destinationImageDescriptor(forSourceImages: [MPSImage], sourceStates: [MPSState]?) -> MPSImageDescriptor

func encode(commandBuffer: any MTLCommandBuffer, primaryImage: MPSImage, secondaryImage: MPSImage, destinationState: AutoreleasingUnsafeMutablePointer&lt;MPSState?>, destinationStateIsTemporary: Bool) -> MPSImage

func encodeBatch(commandBuffer: any MTLCommandBuffer, primaryImages: [MPSImage], secondaryImages: [MPSImage]) -> [MPSImage]

func encodeBatch(commandBuffer: any MTLCommandBuffer, primaryImages: [MPSImage], secondaryImages: [MPSImage], destinationImages: [MPSImage])

func encodeBatch(commandBuffer: any MTLCommandBuffer, primaryImages: [MPSImage], secondaryImages: [MPSImage], destinationStates: AutoreleasingUnsafeMutablePointer&lt;NSArray?>, destinationStateIsTemporary: Bool) -> [MPSImage]

func encodingStorageSize(primaryImage: MPSImage, secondaryImage: MPSImage, sourceStates: [MPSState]?, destinationImage: MPSImage?) -> Int

func isResultStateReusedAcrossBatch() -> Bool

func resultState(primaryImage: MPSImage, secondaryImage: MPSImage, sourceStates: [MPSState]?, destinationImage: MPSImage) -> MPSState?

func resultStateBatch(primaryImage: [MPSImage], secondaryImage: [MPSImage], sourceStates: [[MPSState]]?, destinationImage: [MPSImage]) -> [MPSState]?

func temporaryResultState(commandBuffer: any MTLCommandBuffer, primaryImage: MPSImage, secondaryImage: MPSImage, sourceStates: [MPSState]?, destinationImage: MPSImage) -> MPSState?

func temporaryResultStateBatch(commandBuffer: any MTLCommandBuffer, primaryImage: [MPSImage], secondaryImage: [MPSImage], sourceStates: [[MPSState]]?, destinationImage: [MPSImage]) -> [MPSState]?

## Relationships

### Inherits From

- MPSKernel

## See Also

### Layer Base Classes

class MPSCNNKernel

Base class for neural network layers.

class MPSCNNGradientKernel

The base class for gradient layers.

