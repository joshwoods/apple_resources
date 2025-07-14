

- Accelerate
- BNNS
- BNNS.CropResizeLayer
-  applyBackward(regionOfInterest:outputGradient:generatingInputGradient:filterParameters:) Deprecated

Instance Method

# applyBackward(regionOfInterest:outputGradient:generatingInputGradient:filterParameters:)

Applies a crop-resize filter backward to generate an input gradient.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func applyBackward(
    regionOfInterest: BNNSNDArrayDescriptor,
    outputGradient: BNNSNDArrayDescriptor,
    generatingInputGradient inputGradient: BNNSNDArrayDescriptor,
    filterParameters: BNNSFilterParameters? = nil
) throws
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Applying a Crop-Resize Layer

func apply(input: BNNSNDArrayDescriptor, regionOfInterest: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Applies the layer to a set of input objects, writing the result to a set of output objects.

Deprecated

