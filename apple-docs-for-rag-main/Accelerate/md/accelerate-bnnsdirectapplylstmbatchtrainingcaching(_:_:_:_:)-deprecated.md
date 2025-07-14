

- Accelerate
-  BNNSDirectApplyLSTMBatchTrainingCaching(\_:\_:\_:\_:) Deprecated

Function

# BNNSDirectApplyLSTMBatchTrainingCaching(\_:\_:\_:\_:)

Applies a long short-term memory (LSTM) layer directly to an input.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSDirectApplyLSTMBatchTrainingCaching(
    _ layer_params: UnsafePointer,
    _ filter_params: UnsafePointer?,
    _ training_cache_ptr: UnsafeMutableRawPointer?,
    _ training_cache_capacity: Int
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`layer_params`  

The LSTM layer parameters.

`filter_params`  

Filter runtime parameters.

`training_cache_ptr`  

A pointer to the training cache buffer.

`training_cache_capacity`  

The minimum bytes capacity of the training cache buffer as computed by the training cache capacity function.

## Mentioned in 

Using Long Short-Term Memory Layers (LSTM)

## See Also

### Recurrent layers

Using Long Short-Term Memory Layers (LSTM)

Add long short-term memory (LSTM) layers to recurrent neural networks to avoid long-term dependency problems.

struct BNNSLSTMDataDescriptor

A structure that contains the input-output, hidden, and cell state n-dimensional array descriptors for a long short-term memory (LSTM) layer.

Deprecated

struct BNNSLSTMGateDescriptor

A structure that describes a long short-term memory (LSTM) gate layer.

Deprecated

struct BNNSLayerFlags

Options that control the behavior of a long short-term memory (LSTM) layer.

struct BNNSLayerParametersLSTM

A structure that contains the parameters of a long short-term memory (LSTM) layer.

Deprecated

func BNNSComputeLSTMTrainingCacheCapacity(UnsafePointer&lt;BNNSLayerParametersLSTM>) -> Int

Returns the minimum bytes capacity of the training cache buffer a long short-term memory (LSTM) layer uses when it’s applied.

Deprecated

func BNNSDirectApplyLSTMBatchBackward(UnsafePointer&lt;BNNSLayerParametersLSTM>, UnsafePointer&lt;BNNSLayerParametersLSTM>, UnsafePointer&lt;BNNSFilterParameters>?, UnsafeRawPointer?, Int) -> Int32

Applies a long short-term memory (LSTM) filter backward to generate gradients.

Deprecated

