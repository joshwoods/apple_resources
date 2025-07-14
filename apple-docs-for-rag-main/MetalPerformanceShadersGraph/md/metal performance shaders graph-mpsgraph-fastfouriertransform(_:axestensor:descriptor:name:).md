

- Metal Performance Shaders Graph
- MPSGraph
-  fastFourierTransform(\_:axesTensor:descriptor:name:) 

Instance Method

# fastFourierTransform(\_:axesTensor:descriptor:name:)

Creates a fast Fourier transform operation and returns the result tensor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func fastFourierTransform(
    _ tensor: MPSGraphTensor,
    axesTensor: MPSGraphTensor,
    descriptor: MPSGraphFFTDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

A complex or real-valued input tensor.

`axesTensor`  

A tensor of rank one containing the axes over which MPSGraph performs the transformation. See fastFourierTransform(_:axes:descriptor:name:).

`descriptor`  

A descriptor that defines the parameters of the Fourier transform operation - see MPSGraphFFTDescriptor.

`name`  

The name for the operation.

## Return Value

A valid complex-valued MPSGraphTensor of the same shape as `tensor`.

## Discussion

This operation computes the fast Fourier transform of the input tensor according to the following formulae.

```
    output[mu] = scale * sum_nu exp( +/- i * 2Pi * mu * nu / n ) input[nu], where
```

`scale = 1` for `scaling_mode = none`, `scale = 1/V_f` for `scaling_mode = size`, `scale = 1/sqrt(V_f)` for `scaling_mode = unitary`, where `V_f` is the volume of the transformation defined by the dimensions included in `axes` (`V_f = prod_{i \in axes} shape(input)[i]`) (see scalingMode), `+` is selected in `+/-` when `inverse` is specified, otherwise `-` is used and the sum is done separately over each dimension in `axes` and `n` is the dimension length of that axis.

Tip

Currently MPSGraph supports the transformation only within the last four dimensions of the input tensor. In case you need to transform higher dimensions than the last four, you can tranpose the higher dimensions of the input with transpose(_:permutation:name:) to be within that last four and then transpose the result tensor back with the inverse of the input transpose.

