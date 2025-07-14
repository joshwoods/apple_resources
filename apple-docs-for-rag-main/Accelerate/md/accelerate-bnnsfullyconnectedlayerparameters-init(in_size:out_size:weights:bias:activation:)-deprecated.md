

- Accelerate
- BNNSFullyConnectedLayerParameters
-  init(in_size:out_size:weights:bias:activation:) Deprecated

Initializer

# init(in_size:out_size:weights:bias:activation:)

Returns a new fully connected layer parameters structure.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.12–11.0DeprecatedtvOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
init(
    in_size: Int,
    out_size: Int,
    weights: BNNSLayerData,
    bias: BNNSLayerData,
    activation: BNNSActivation
)
```

## Parameters 

`in_size`  

The size of the input vector.

`out_size`  

The size of the output vector.

`weights`  

Matrix coefficients, containing in_size `*` out_size values.

`bias`  

Layer bias, containing out_size values, one for each output component.

`activation`  

The layer activation function.

## See Also

### Initializers

init()Deprecated

init(in_size: Int, out_size: Int, weights: BNNSLayerData)Deprecated

