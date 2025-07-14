

- Accelerate
- BNNS
- BNNS.CropResizeLayer
-  apply(input:regionOfInterest:output:filterParameters:) Deprecated

Instance Method

# apply(input:regionOfInterest:output:filterParameters:)

Applies the layer to a set of input objects, writing the result to a set of output objects.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+Mac Catalyst

``` source
func apply(
    input: BNNSNDArrayDescriptor,
    regionOfInterest: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    filterParameters: BNNSFilterParameters? = nil
) throws
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Applying a Crop-Resize Layer

func applyBackward(regionOfInterest: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Applies a crop-resize filter backward to generate an input gradient.

Deprecated

