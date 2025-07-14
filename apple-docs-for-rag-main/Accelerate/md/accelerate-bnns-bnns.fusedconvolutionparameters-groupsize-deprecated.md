

- Accelerate
- BNNS
- BNNS.FusedConvolutionParameters
-  groupSize Deprecated

Instance Property

# groupSize

The convolution group size.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var groupSize: Int
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Inspecting the Properties of a Fused Convolution Parameters Structure

var type: BNNS.ConvolutionType

An enumeration that specifies the convolution type.

Deprecated

var weights: BNNSNDArrayDescriptor

The descriptor of the weights.

Deprecated

var bias: BNNSNDArrayDescriptor?

The descriptor of the bias.

Deprecated

var stride: (x: Int, y: Int)

The width and height increments of the input image.

Deprecated

var dilationStride: (x: Int, y: Int)

The width and height increments between elements in the input image during convolution.

Deprecated

var padding: BNNS.ConvolutionPadding

The number of zeros that the operation virtually adds to the edges of the input.

Deprecated

