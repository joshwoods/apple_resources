

- Metal Performance Shaders
-  MPSCNNConvolutionTransposeGradient 

Class

# MPSCNNConvolutionTransposeGradient

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MPSCNNConvolutionTransposeGradient : MPSCNNGradientKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, weights: any MPSCNNConvolutionDataSource)

### Instance Properties

var dataSource: any MPSCNNConvolutionDataSource

var gradientOption: MPSCNNConvolutionGradientOption

var groups: Int

var sourceGradientFeatureChannels: Int

var sourceImageFeatureChannels: Int

### Instance Methods

func reloadWeightsAndBiases(with: any MTLCommandBuffer, state: MPSCNNConvolutionWeightsAndBiasesState)

func reloadWeightsAndBiasesFromDataSource()

## Relationships

### Inherits From

- MPSCNNGradientKernel

