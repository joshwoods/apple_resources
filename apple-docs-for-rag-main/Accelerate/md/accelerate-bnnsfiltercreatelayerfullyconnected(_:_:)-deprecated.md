

- Accelerate
-  BNNSFilterCreateLayerFullyConnected(\_:\_:) Deprecated

Function

# BNNSFilterCreateLayerFullyConnected(\_:\_:)

Returns a new fully connected layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterCreateLayerFullyConnected(
    _ layer_params: UnsafePointer,
    _ filter_params: UnsafePointer?
) -> BNNSFilter?
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`layer_params`  

Layer parameters.

`filter_params`  

Filter runtime parameters.

## Discussion

Use a fully connected layer to construct each output feature from a linear combination of all input features. Fully connected layers compute the matrix-vector product of a weights matrix and the input vector.

### Applying a Fully Connected Filter With a 2D Weights Matrix

In the case where your input data is a vector and your weights data is a matrix, provide the weights as an *m x n* row-major matrix where *m* is the number of fully connected results, and *n* is the number of items in the input.

For example, the following code defines a column matrix input that contains four values, a 3 x 4 weights matrix, and a three-element vector that receives the result:

```
let input: [Float] = [1,
                      2,
                      3,
                      4]

let weightsData: [Float] = [10, 20, 30, 40,
                            100, 200, 300, 400,
                            1000, 2000, 3000, 4000]

let n = 3

var output = [Float](repeating: .nan,
                     count: n)
```

Use the following code to create and apply the fully connected layer:

```
let flags = BNNSNDArrayFlags(0)

weightsData.withUnsafeBufferPointer { weightsPtr in
    let inDescription = BNNSNDArrayDescriptor(flags: flags,
                                              layout: BNNSDataLayoutVector,
                                              size: (4, 0, 0, 0, 0, 0, 0, 0),
                                              stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                              data: nil,
                                              data_type: .float,
                                              table_data: nil,
                                              table_data_type: .float,
                                              data_scale: 0,
                                              data_bias: 0)

    let outDescription = BNNSNDArrayDescriptor(flags: flags,
                                               layout: BNNSDataLayoutVector,
                                               size: (3, 0, 0, 0, 0, 0, 0, 0),
                                               stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                               data: nil,
                                               data_type: .float,
                                               table_data: nil,
                                               table_data_type: .float,
                                               data_scale: 0,
                                               data_bias: 0)

    let weightsDescription = BNNSNDArrayDescriptor(flags: flags,
                                                   layout: BNNSDataLayoutRowMajorMatrix,
                                                   size: (4, 3, 0, 0, 0, 0, 0, 0),
                                                   stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                   data: UnsafeMutableRawPointer(mutating: weightsPtr.baseAddress),
                                                   data_type: .float,
                                                   table_data: nil,
                                                   table_data_type: .float,
                                                   data_scale: 0,
                                                   data_bias: 0)

    var layerParameters = BNNSLayerParametersFullyConnected(i_desc: inDescription,
                                                            w_desc: weightsDescription,
                                                            o_desc: outDescription,
                                                            bias: BNNSNDArrayDescriptor(),
                                                            activation: .identity)

    let filter = BNNSFilterCreateLayerFullyConnected(&layerParameters,
                                                     nil)
    defer {
        BNNSFilterDestroy(filter)
    }

    BNNSFilterApply(filter,
                    input,
                    &output)
}
```

On return, `output` contains the following values:

```
[300.0,      // 1 * 10 + 2 * 20 + 3 * 30 + 4 * 40
 3000.0,     // 1 * 100 + 2 * 200 + 3 * 300 + 4 * 400
 30000.0]    // 1 * 1000 + 2 * 2000 + 3 * 3000 + 4 * 4000
```

## See Also

### Fully connected layers

struct BNNSFullyConnectedLayerParameters

A structure containing fully connected layer parameters.

Deprecated

func BNNSFilterCreateFullyConnectedLayer(UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSFullyConnectedLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a fully connected filter, initialized with input, output, layer, and filter parameters.

Deprecated

class FullyConnectedLayer

A layer object that wraps a fully connected filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersFullyConnected

A structure that contains the parameters of a fully connected layer.

Deprecated

