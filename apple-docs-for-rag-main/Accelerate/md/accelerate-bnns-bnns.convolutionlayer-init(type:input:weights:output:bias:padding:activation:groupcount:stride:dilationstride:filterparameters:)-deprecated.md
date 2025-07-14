

- Accelerate
- BNNS
- BNNS.ConvolutionLayer
-  init(type:input:weights:output:bias:padding:activation:groupCount:stride:dilationStride:filterParameters:) Deprecated

Initializer

# init(type:input:weights:output:bias:padding:activation:groupCount:stride:dilationStride:filterParameters:)

Returns a new convolution layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
convenience init?(
    type convolutionType: BNNS.ConvolutionType,
    input: BNNSNDArrayDescriptor,
    weights: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    bias: BNNSNDArrayDescriptor?,
    padding: BNNS.ConvolutionPadding,
    activation: BNNS.ActivationFunction,
    groupCount: Int,
    stride: (x: Int, y: Int),
    dilationStride: (x: Int, y: Int),
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`convolutionType`  

An enumeration that specifies the convolution type.

`input`  

The descriptor of the input. The data type of the input must be BNNSDataLayoutImageCHW.

`weights`  

The descriptor of the weights. The data type of the weights must be BNNSDataLayoutConvolutionWeightsOIHW, BNNSDataLayoutConvolutionWeightsOIHrWr, BNNSDataLayoutConvolutionWeightsIOHrWr, or BNNSDataLayoutConvolutionWeightsOIHW_Pack32.

`output`  

The descriptor of the output. The data type of the output must be BNNSDataLayoutImageCHW.

`bias`  

The descriptor of the bias.

`padding`  

The padding, which is the number of virtual zeros added to the sides of each channel.

`activation`  

The activation function that the layer applies to the output.

`groupCount`  

The number of convolution groups.

`stride`  

The width and height increments of the input image.

`dilationStride`  

The width and height increments between elements in the input image during convolution.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

Convolution layers only support arrays with a data type of `float`, `float16`, `int8`, or `uint8`.

