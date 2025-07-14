

- Metal Performance Shaders
-  MPSNDArrayBinaryKernel 

Class

# MPSNDArrayBinaryKernel

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MPSNDArrayBinaryKernel : MPSNDArrayMultiaryKernel
```

## Topics

### Initializers

init(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Instance Properties

var primaryDilationRates: MPSNDArraySizesDeprecated

var primaryEdgeMode: MPSImageEdgeModeDeprecated

var primaryKernelSizes: MPSNDArraySizesDeprecated

var primaryOffsets: MPSNDArrayOffsetsDeprecated

var primaryStrides: MPSNDArrayOffsetsDeprecated

var secondaryDilationRates: MPSNDArraySizesDeprecated

var secondaryEdgeMode: MPSImageEdgeModeDeprecated

var secondaryKernelSizes: MPSNDArraySizesDeprecated

var secondaryOffsets: MPSNDArrayOffsetsDeprecated

var secondaryStrides: MPSNDArrayOffsetsDeprecated

### Instance Methods

func encode(to: any MTLCommandBuffer, primarySourceArray: MPSNDArray, secondarySourceArray: MPSNDArray) -> MPSNDArray

func encode(to: any MTLCommandBuffer, primarySourceArray: MPSNDArray, secondarySourceArray: MPSNDArray, destinationArray: MPSNDArray)

func encode(to: any MTLCommandBuffer, primarySourceArray: MPSNDArray, secondarySourceArray: MPSNDArray, resultState: MPSState?, destinationArray: MPSNDArray)

func encode(to: any MTLCommandBuffer, primarySourceArray: MPSNDArray, secondarySourceArray: MPSNDArray, resultState: AutoreleasingUnsafeMutablePointer&lt;MPSState?>?, outputStateIsTemporary: Bool) -> MPSNDArray

## Relationships

### Inherits From

- MPSNDArrayMultiaryKernel

