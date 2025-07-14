

- Accelerate
-  BNNSFilterCreateConvolutionLayer(\_:\_:\_:\_:) Deprecated

Function

# BNNSFilterCreateConvolutionLayer(\_:\_:\_:\_:)

Returns a convolution filter, initialized with input, output, layer, and filter parameters.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.12–11.0DeprecatedtvOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
func BNNSFilterCreateConvolutionLayer(
    _ in_desc: UnsafePointer,
    _ out_desc: UnsafePointer,
    _ layer_params: UnsafePointer,
    _ filter_params: UnsafePointer?
) -> BNNSFilter?
```

Deprecated

Use BNNSFilterCreateLayerConvolution(_:_:) instead.

## Parameters 

`in_desc`  

Pointer to a `BNNSImageStackDescriptor` struct describing the input

`out_desc`  

Pointer to a `BNNSImageStackDescriptor` struct describing the output

`layer_params`  

Pointer to a `BNNSConvolutionLayerParameters` struct describing the layer parameters

`filter_params`  

Pointer to a `BNNSFilterParameters` struct describing the filter parameters

## Return Value

A BNNSFilter object representing a convolution filter configured with the specified parameters

## See Also

### Convolution layers

struct BNNSConvolutionLayerParameters

A structure containing convolution parameters.

Deprecated

class ConvolutionLayer

A layer object that wraps a convolution filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersConvolution

A structure that contains the parameters of a convolution layer.

Deprecated

func BNNSFilterCreateLayerConvolution(UnsafePointer&lt;BNNSLayerParametersConvolution>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new convolution layer.

Deprecated

func BNNSFilterCreateLayerTransposedConvolution(UnsafePointer&lt;BNNSLayerParametersConvolution>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new transposed convolution layer.

Deprecated

