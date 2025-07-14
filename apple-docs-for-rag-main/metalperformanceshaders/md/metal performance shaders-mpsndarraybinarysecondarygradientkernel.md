

- Metal Performance Shaders
-  MPSNDArrayBinarySecondaryGradientKernel 

Class

# MPSNDArrayBinarySecondaryGradientKernel

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MPSNDArrayBinarySecondaryGradientKernel : MPSNDArrayMultiaryGradientKernel
```

## Topics

### Initializers

init(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Instance Methods

func encode(to: any MTLCommandBuffer, primarySourceArray: MPSNDArray, secondarySourceArray: MPSNDArray, sourceGradient: MPSNDArray, gradientState: MPSState) -> MPSNDArray

func encode(to: any MTLCommandBuffer, primarySourceArray: MPSNDArray, secondarySourceArray: MPSNDArray, sourceGradient: MPSNDArray, gradientState: MPSState, destinationArray: MPSNDArray)

## Relationships

### Inherits From

- MPSNDArrayMultiaryGradientKernel

