

- Accelerate
-  BNNSPoolingFilterApplyBatchEx(\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSPoolingFilterApplyBatchEx(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a pooling filter to a set of input objects with support for multiple data types for indices.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSPoolingFilterApplyBatchEx(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ in: UnsafeRawPointer,
    _ in_stride: Int,
    _ out: UnsafeMutableRawPointer,
    _ out_stride: Int,
    _ indices_data_type: BNNSDataType,
    _ indices: UnsafeMutableRawPointer?,
    _ idx_stride: Int
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`filter`  

The filter to apply.

`batch_size`  

The number of input-output pairs.

`in`  

A pointer to the input data.

`in_stride`  

The increment, in values, between inputs.

`out`  

A pointer to the output data.

`out_stride`  

The increment, in values, between outputs.

`indices_data_type`  

The data type of the indices data.

`indices`  

A pointer to the indices data.

`idx_stride`  

The increment, in values, between indices.

## Discussion

This function is an extension to BNNSPoolingFilterApplyBatch(_:_:_:_:_:_:_:_:) that supports 32- and 64-bit unsigned-integer indices for max pooling and unpooling.

## See Also

### Pooling layers

struct BNNSPoolingLayerParameters

A structure containing pooling layer parameters.

Deprecated

func BNNSFilterCreatePoolingLayer(UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSPoolingLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a pooling filter, initialized with input, output, layer, and filter parameters.

Deprecated

class PoolingLayer

A layer object that wraps a pooling filter and manages its deinitialization.

Deprecated

struct BNNSPoolingFunction

Constants that describe pooling functions.

var BNNSPoolingFunctionAverage: BNNSPoolingFunctionDeprecated

var BNNSPoolingFunctionMax: BNNSPoolingFunctionDeprecated

struct BNNSLayerParametersPooling

A structure that contains the parameters of a pooling layer.

Deprecated

func BNNSFilterCreateLayerPooling(UnsafePointer&lt;BNNSLayerParametersPooling>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new pooling layer.

Deprecated

func BNNSPoolingFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, UnsafeMutablePointer&lt;Int>?, Int) -> Int32

Applies a pooling filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSPoolingFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafePointer&lt;Int>?, Int) -> Int32

Applies a pooling filter backward to generate gradients.

Deprecated

func BNNSPoolingFilterApplyBackwardBatchEx(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, BNNSDataType, UnsafeRawPointer?, Int) -> Int32

Applies a pooling filter backward to generate gradients with support for multiple data types for indices.

Deprecated

