

- ML Compute
- MLCTensor
-  dequantized(to:scale:zeroPoint:) Deprecated

Instance Method

# dequantized(to:scale:zeroPoint:)

Converts a tensor you quantize to a 32-bit floating-point tensor.

iOS 15.0–17.4DeprecatediPadOS 15.0–17.4DeprecatedMac Catalyst 15.0–17.4DeprecatedmacOS 12.0–14.3DeprecatedtvOS 15.0–17.4Deprecated

``` source
func dequantized(
    to type: MLCDataType,
    scale: MLCTensor,
    zeroPoint bias: MLCTensor
) -> MLCTensor?
```

## Parameters 

`type`  

The tensor data type.

`scale`  

The scale the system uses when quantizing the data.

`bias`  

The offset value the system uses when quantizing the data.

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

func dequantized(to: MLCDataType, scale: MLCTensor, bias: MLCTensor, axis: Int) -> MLCTensor?

Converts a tensor you quantize to a 32-bit floating-point tensor.

Deprecated

