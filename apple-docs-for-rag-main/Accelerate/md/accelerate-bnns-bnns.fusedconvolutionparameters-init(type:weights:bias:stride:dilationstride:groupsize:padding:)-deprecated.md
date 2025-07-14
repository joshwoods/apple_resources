

- Accelerate
- BNNS
- BNNS.FusedConvolutionParameters
-  init(type:weights:bias:stride:dilationStride:groupSize:padding:) Deprecated

Initializer

# init(type:weights:bias:stride:dilationStride:groupSize:padding:)

Returns a new fused convolution parameters structure.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
init(
    type: BNNS.ConvolutionType,
    weights: BNNSNDArrayDescriptor,
    bias: BNNSNDArrayDescriptor?,
    stride: (x: Int, y: Int),
    dilationStride: (x: Int, y: Int),
    groupSize: Int,
    padding: BNNS.ConvolutionPadding
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`type`  

An enumeration that specifies the convolution type.

`weights`  

The descriptor of the weights.

`bias`  

The descriptor of the bias.

`stride`  

The width and height increments of the input image.

`dilationStride`  

The width and height increments between elements in the input image during convolution.

`groupSize`  

The convolution group size.

`padding`  

The number of zeros that the operation virtually adds to the edges of the input.

