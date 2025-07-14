

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNBinaryConvolution 

Class

# MPSCNNBinaryConvolution

A convolution kernel with binary weights and an input image using binary approximations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSCNNBinaryConvolution : MPSCNNKernel
```

## Overview

The `MPSCNNBinaryConvolution` optionally first binarizes the input image and then convolves the result with a set of binary-valued filters, each producing one feature map in the output image (which is a normal image).

The output is computed as follows:

where the *sum over* *dx,dy* is over the spatial filter kernel window defined by kernelWidth and kernelHeight, *sum over* *f* is over the input feature channel indices within group, *B* contains the binary weights, interpreted as `{-1, 1}` or `{0, 1}` and *scale\[c\]* is the `outputScaleTerms` array and bias is the `outputBiasTerms` array. Above *i* is the image index in batch the sum over input channels *f* runs through the group indices. The convolution operator ⊗ is defined by MPSCNNBinaryConvolutionType passed in at initialization time of the filter:

MPSCNNBinaryConvolutionType.binaryWeights  
The input image is not binarized at all and the convolution is computed interpreting the weights as `[0, 1] -> {-1, 1}` with the given scaling terms.

MPSCNNBinaryConvolutionType.XNOR  
The convolution is computed by first binarizing the input image using the sign function `bin(x) = x MPSCNNBinaryConvolutionType.AND  
The convolution is computed by first binarizing the input image using the sign function `bin(x) = x 

where *(dx,dy)* are summed over the convolution filter window.

where *in* is the original input image (in full precision) and *Nc* is the number of input channels in the input image. Parameter `beta` is not passed as input and to enable beta-scaling the user can provide MPSCNNBinaryConvolutionFlags.useBetaScaling in the flags parameter in the initialization functions.

Finally the normal activation neuron is applied and the result is written to the output image.

Note

`MPSCNNBinaryConvolution` does not currently support groups greater than 1.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, convolutionData: any MPSCNNConvolutionDataSource, outputBiasTerms: UnsafePointer&lt;Float>?, outputScaleTerms: UnsafePointer&lt;Float>?, inputBiasTerms: UnsafePointer&lt;Float>?, inputScaleTerms: UnsafePointer&lt;Float>?, type: MPSCNNBinaryConvolutionType, flags: MPSCNNBinaryConvolutionFlags)

Initializes a binary convolution kernel.

init(device: any MTLDevice, convolutionData: any MPSCNNConvolutionDataSource, scaleValue: Float, type: MPSCNNBinaryConvolutionType, flags: MPSCNNBinaryConvolutionFlags)

Initializes a binary convolution kernel.

protocol MPSCNNConvolutionDataSource

The protocol that provides convolution filter weights and bias terms.

enum MPSCNNBinaryConvolutionType

Options that defines what operations are used to perform binary convolution.

enum MPSCNNBinaryConvolutionFlags

Options used to control binary convolution kernels.

### Instance Properties

var inputFeatureChannels: Int

var outputFeatureChannels: Int

## Relationships

### Inherits From

- MPSCNNKernel

## See Also

### Convolution Layers

class MPSCNNConvolution

A convolution kernel that convolves the input image with a set of filters, with each producing one feature map in the output image.

class MPSCNNDepthWiseConvolutionDescriptor

A description of a convolution object that does depthwise convolution.

class MPSCNNSubPixelConvolutionDescriptor

A description of a convolution object that does subpixel upsampling and reshaping.

class MPSCNNConvolutionTranspose

A transposed convolution kernel.

class MPSCNNConvolutionGradient

A gradient convolution kernel.

class MPSCNNConvolutionGradientState

An object that exposes a gradient convolution kernel's gradient with respect to weights and biases.

protocol MPSImageSizeEncodingState

A protocol for objects that contain information about an image size elsewhere in the graph.

class MPSCNNConvolutionWeightsAndBiasesState

A class that stores weights and biases.

