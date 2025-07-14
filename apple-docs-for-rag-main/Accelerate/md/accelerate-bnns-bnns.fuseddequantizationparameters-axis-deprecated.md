

- Accelerate
- BNNS
- BNNS.FusedDequantizationParameters
-  axis Deprecated

Instance Property

# axis

The index of the axis on which the function applies scale and bias.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var axis: Int?
```

Deprecated

Use the BNNSGraph API instead.

## Discussion

Set to `nil` to dequantize the entire tensor using scale and bias.

## See Also

### Inspecting the Properties of a Fused Dequantization Parameters Structure

var scale: BNNSNDArrayDescriptor?

The descriptor of the scale.

Deprecated

var bias: BNNSNDArrayDescriptor?

The descriptor of the bias.

Deprecated

