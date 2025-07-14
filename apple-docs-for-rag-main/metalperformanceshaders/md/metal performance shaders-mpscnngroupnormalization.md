

- Metal Performance Shaders
-  MPSCNNGroupNormalization 

Class

# MPSCNNGroupNormalization

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MPSCNNGroupNormalization : MPSCNNKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, dataSource: any MPSCNNGroupNormalizationDataSource)

### Instance Properties

var dataSource: any MPSCNNGroupNormalizationDataSource

var epsilon: Float

### Instance Methods

func reloadGammaAndBeta(with: any MTLCommandBuffer, gammaAndBetaState: MPSCNNNormalizationGammaAndBetaState)

func reloadGammaAndBetaFromDataSource()

func resultState(sourceImage: MPSImage, sourceStates: [MPSState]?, destinationImage: MPSImage) -> MPSCNNGroupNormalizationGradientState?

func temporaryResultState(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage, sourceStates: [MPSState]?, destinationImage: MPSImage) -> MPSCNNGroupNormalizationGradientState?

## Relationships

### Inherits From

- MPSCNNKernel

