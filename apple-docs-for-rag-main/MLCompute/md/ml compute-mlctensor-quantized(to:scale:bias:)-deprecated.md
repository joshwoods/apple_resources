

- ML Compute
- MLCTensor
-  quantized(to:scale:bias:) Deprecated

Instance Method

# quantized(to:scale:bias:)

Converts a 32-bit floating-point tensor with the scale and bias you specify.

iOS 15.0–17.4DeprecatediPadOS 15.0–17.4DeprecatedMac Catalyst 15.0–17.4DeprecatedmacOS 12.0–14.3DeprecatedtvOS 15.0–17.4Deprecated

``` source
func quantized(
    to type: MLCDataType,
    scale: Float,
    bias: Int
) -> MLCTensor?
```

## Parameters 

`type`  

The tensor data type.

`scale`  

The scale to apply for quantizing.

`bias`  

The offset value that maps to float zero.

## Return Value

A tensor the system quantizes.

## Discussion

Important

The tensor type must be MLCDataType.int8, MLCDataType.uint8, or MLCDataType.int32.

## See Also

### Converting Tensors

func quantized(to: MLCDataType, scale: MLCTensor, bias: MLCTensor, axis: Int) -> MLCTensor?

Converts a 32-bit floating-point tensor with the scale and bias you specify.

Deprecated

func dequantized(to: MLCDataType, scale: MLCTensor, zeroPoint: MLCTensor) -> MLCTensor?

Converts a tensor you quantize to a 32-bit floating-point tensor.

Deprecated

func dequantized(to: MLCDataType, scale: MLCTensor, bias: MLCTensor, axis: Int) -> MLCTensor?

Converts a tensor you quantize to a 32-bit floating-point tensor.

Deprecated

