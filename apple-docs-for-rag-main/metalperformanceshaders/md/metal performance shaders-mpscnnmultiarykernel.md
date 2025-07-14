

- Metal Performance Shaders
-  MPSCNNMultiaryKernel 

Class

# MPSCNNMultiaryKernel

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MPSCNNMultiaryKernel : MPSKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, sourceCount: Int)

### Instance Properties

var clipRect: MTLRegion

var destinationFeatureChannelOffset: Int

var destinationImageAllocator: any MPSImageAllocator

var isBackwards: Bool

var isStateModified: Bool

var padding: any MPSNNPadding

var sourceCount: Int

### Instance Methods

func appendBatchBarrier() -> Bool

func destinationImageDescriptor(sourceImages: [MPSImage], sourceStates: [MPSState]?) -> MPSImageDescriptor

func dilationRateXatIndex(Int) -> Int

func dilationRateYatIndex(Int) -> Int

func edgeMode(at: Int) -> MPSImageEdgeMode

func encode(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage]) -> MPSImage

func encode(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage], destinationImage: MPSImage)

func encode(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage], destinationState: AutoreleasingUnsafeMutablePointer&lt;MPSState?>, destinationStateIsTemporary: Bool) -> MPSImage

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [[MPSImage]]) -> [MPSImage]

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [[MPSImage]], destinationImages: [MPSImage])

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [[MPSImage]], destinationStates: AutoreleasingUnsafeMutablePointer&lt;NSArray?>, destinationStateIsTemporary: Bool) -> [MPSImage]

func isResultStateReusedAcrossBatch() -> Bool

func kernelHeight(at: Int) -> Int

func kernelWidth(at: Int) -> Int

func offset(at: Int) -> MPSOffset

func resultState(sourceImages: [MPSImage], sourceStates: [MPSState]?, destinationImage: MPSImage) -> MPSState?

func resultStateBatch(sourceImages: [[MPSImage]], sourceStates: [[MPSState]]?, destinationImage: [MPSImage]) -> [MPSState]?

func setDilationRateX(Int, at: Int)

func setDilationRateY(Int, at: Int)

func setEdgeMode(MPSImageEdgeMode, at: Int)

func setKernelHeight(Int, at: Int)

func setKernelWidth(Int, at: Int)

func setOffset(MPSOffset, at: Int)

func setSourceFeatureChannelMaxCount(Int, at: Int)

func setSourceFeatureChannelOffset(Int, at: Int)

func setStrideInPixelsX(Int, at: Int)

func setStrideInPixelsY(Int, at: Int)

func sourceFeatureChannelMaxCount(at: Int) -> Int

func sourceFeatureChannelOffset(at: Int) -> Int

func stride(inPixelsXatIndex: Int) -> Int

func stride(inPixelsYatIndex: Int) -> Int

func temporaryResultState(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage], sourceStates: [MPSState]?, destinationImage: MPSImage) -> MPSState?

func temporaryResultStateBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [[MPSImage]], sourceStates: [[MPSState]]?, destinationImage: [MPSImage]) -> [MPSState]?

## Relationships

### Inherits From

- MPSKernel

