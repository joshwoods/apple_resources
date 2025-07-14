

- Accelerate
-  BNNSFilterCreateFullyConnectedLayer(\_:\_:\_:\_:) Deprecated

Function

# BNNSFilterCreateFullyConnectedLayer(\_:\_:\_:\_:)

Returns a fully connected filter, initialized with input, output, layer, and filter parameters.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.12–11.0DeprecatedtvOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
func BNNSFilterCreateFullyConnectedLayer(
    _ in_desc: UnsafePointer,
    _ out_desc: UnsafePointer,
    _ layer_params: UnsafePointer,
    _ filter_params: UnsafePointer?
) -> BNNSFilter?
```

Deprecated

Use BNNSFilterCreateFullyConnectedLayer(_:_:_:_:) instead.

## Parameters 

`in_desc`  

Pointer to a `BNNSVectorDescriptor` struct describing the input

`out_desc`  

Pointer to a `BNNSVectorDescriptor` struct describing the output

`layer_params`  

Pointer to a `BNNSFullyConnectedLayerParameters` struct describing the layer parameters

`filter_params`  

Pointer to a `BNNSFilterParameters` struct describing the filter parameters

## Return Value

A BNNSFilter object representing a fully connected filter configured with the specified parameters

## See Also

### Fully connected layers

struct BNNSFullyConnectedLayerParameters

A structure containing fully connected layer parameters.

Deprecated

class FullyConnectedLayer

A layer object that wraps a fully connected filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersFullyConnected

A structure that contains the parameters of a fully connected layer.

Deprecated

func BNNSFilterCreateLayerFullyConnected(UnsafePointer&lt;BNNSLayerParametersFullyConnected>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new fully connected layer.

Deprecated

