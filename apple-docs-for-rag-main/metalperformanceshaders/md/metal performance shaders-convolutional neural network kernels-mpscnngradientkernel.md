

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNGradientKernel 

Class

# MPSCNNGradientKernel

The base class for gradient layers.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.0+macOS 10.13.4+tvOS 11.3+visionOS 1.0+

``` source
class MPSCNNGradientKernel : MPSCNNBinaryKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Instance Properties

var kernelOffsetX: Int

var kernelOffsetY: Int

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, sourceGradient: MPSImage, sourceImage: MPSImage, gradientState: MPSState) -> MPSImage

func encode(commandBuffer: any MTLCommandBuffer, sourceGradient: MPSImage, sourceImage: MPSImage, gradientState: MPSState, destinationGradient: MPSImage)

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceGradients: [MPSImage], sourceImages: [MPSImage], gradientStates: [MPSState]) -> [MPSImage]

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceGradients: [MPSImage], sourceImages: [MPSImage], gradientStates: [MPSState], destinationGradients: [MPSImage])

## Relationships

### Inherits From

- MPSCNNBinaryKernel

## See Also

### Layer Base Classes

class MPSCNNKernel

Base class for neural network layers.

class MPSCNNBinaryKernel

A convolution neural network kernel.

