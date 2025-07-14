

- ML Compute
- MLCTensor
-  dequantized(to:scale:bias:axis:) Deprecated

Instance Method

# dequantized(to:scale:bias:axis:)

Converts a tensor you quantize to a 32-bit floating-point tensor.

iOS 15.0–17.4DeprecatediPadOS 15.0–17.4DeprecatedMac Catalyst 15.0–17.4DeprecatedmacOS 12.0–14.3DeprecatedtvOS 15.0–17.4Deprecated

``` source
func dequantized(
    to type: MLCDataType,
    scale: MLCTensor,
    bias: MLCTensor,
    axis: Int
) -> MLCTensor?
```

## Parameters 

`type`  

The tensor data type.

`scale`  

The scale the system uses when quantizing the data.

`bias`  

The offset value the system uses when quantizing the data.

`axis`  

The dimension on which to apply per-channel quantization.

## Return Value

A tensor the system dequantizes.

## Discussion

Important

The tensor type must be MLCDataType.float32.

## See Also

### Converting Tensors

func quantized(to: MLCDataType, scale: Float, bias: Int) -> MLCTensor?

Converts a 32-bit floating-point tensor with the scale and bias you specify.

Deprecated

func quantized(to: MLCDataType, scale: MLCTensor, bias: MLCTensor, axis: Int) -> MLCTensor?

Converts a 32-bit floating-point tensor with the scale and bias you specify.

Deprecated

func dequantized(to: MLCDataType, scale: MLCTensor, zeroPoint: MLCTensor) -> MLCTensor?

Converts a tensor you quantize to a 32-bit floating-point tensor.

Deprecated

