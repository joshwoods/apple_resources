

- Accelerate
-  BNNSPoolingFilterApplyBackwardBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSPoolingFilterApplyBackwardBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a pooling filter backward to generate gradients.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSPoolingFilterApplyBackwardBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ in: UnsafeRawPointer?,
    _ in_stride: Int,
    _ in_delta: UnsafeMutablePointer?,
    _ in_delta_stride: Int,
    _ out: UnsafeRawPointer?,
    _ out_stride: Int,
    _ out_delta: UnsafeMutablePointer,
    _ out_delta_stride: Int,
    _ bias_delta: UnsafeMutablePointer?,
    _ indices: UnsafePointer?,
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

Pointer to input object.

`in_stride`  

Increment, in values, between input objects.

`in_delta`  

The descriptor of the input delta.

`in_delta_stride`  

Increment, in values, between input delta objects.

`out`  

Pointer to output object.

`out_stride`  

Increment, in values, between output objects.

`out_delta`  

The descriptor of the output delta.

`out_delta_stride`  

Increment, in values, between output delta objects.

`bias_delta`  

The descriptor of the bias delta.

`indices`  

Pointer to indices object.

`idx_stride`  

Increment, in values, between indices objects.

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

func BNNSPoolingFilterApplyBatchEx(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, BNNSDataType, UnsafeMutableRawPointer?, Int) -> Int32

Applies a pooling filter to a set of input objects with support for multiple data types for indices.

Deprecated

func BNNSPoolingFilterApplyBackwardBatchEx(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, BNNSDataType, UnsafeRawPointer?, Int) -> Int32

Applies a pooling filter backward to generate gradients with support for multiple data types for indices.

Deprecated

