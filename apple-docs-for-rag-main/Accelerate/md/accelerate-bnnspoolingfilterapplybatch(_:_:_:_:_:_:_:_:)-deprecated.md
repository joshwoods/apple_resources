

- Accelerate
-  BNNSPoolingFilterApplyBatch(\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSPoolingFilterApplyBatch(\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a pooling filter to a set of input objects, writing the result to a set of output objects.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSPoolingFilterApplyBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ in: UnsafeRawPointer,
    _ in_stride: Int,
    _ out: UnsafeMutableRawPointer,
    _ out_stride: Int,
    _ indices: UnsafeMutablePointer?,
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

Pointer to the input data.

`in_stride`  

Increment, in values, between inputs.

`out`  

Increment, in values, between outputs.

`out_stride`  

Increment, in values, between outputs.

`indices`  

The indices to user.

`idx_stride`  

Increment, in values, between indices.

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

func BNNSPoolingFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafePointer&lt;Int>?, Int) -> Int32

Applies a pooling filter backward to generate gradients.

Deprecated

func BNNSPoolingFilterApplyBatchEx(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, BNNSDataType, UnsafeMutableRawPointer?, Int) -> Int32

Applies a pooling filter to a set of input objects with support for multiple data types for indices.

Deprecated

func BNNSPoolingFilterApplyBackwardBatchEx(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, BNNSDataType, UnsafeRawPointer?, Int) -> Int32

Applies a pooling filter backward to generate gradients with support for multiple data types for indices.

Deprecated

