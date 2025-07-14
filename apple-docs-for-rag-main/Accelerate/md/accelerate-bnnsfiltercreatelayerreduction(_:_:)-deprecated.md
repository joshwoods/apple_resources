

- Accelerate
-  BNNSFilterCreateLayerReduction(\_:\_:) Deprecated

Function

# BNNSFilterCreateLayerReduction(\_:\_:)

Returns a new reduction layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterCreateLayerReduction(
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

The filter runtime parameters.

## Discussion

Use a reduction layer to reduce an axis or axes of a tensor to a scalar value. Specify a size of one for the dimension or dimensions you need to reduce.

For example, given the following source data and n-dimensional array descriptors:

```
let sourceData: [Float] = [1, 4, 7,
                           2, 5, 8,
                           3, 6, 9]

let inDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                         layout: BNNSDataLayoutRowMajorMatrix,
                                         size: (3, 3, 0, 0, 0, 0, 0, 0),
                                         stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                         data: nil,
                                         data_type: .float,
                                         table_data: nil,
                                         table_data_type: .float,
                                         data_scale: 0,
                                         data_bias: 0)

var outDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                          layout: BNNSDataLayoutRowMajorMatrix,
                                          size: (0, 0, 0, 0, 0, 0, 0, 0),
                                          stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                          data: nil,
                                          data_type: .float,
                                          table_data: nil,
                                          table_data_type: .float,
                                          data_scale: 0,
                                          data_bias: 0)
```

Use the following code to compute the sums of elements of each row:

```
outDescriptor.size = (1, 3, 0, 0, 0, 0, 0, 0)

var layerParams = BNNSLayerParametersReduction(i_desc: inDescriptor,
                                               o_desc: outDescriptor,
                                               w_desc: BNNSNDArrayDescriptor(),
                                               reduce_func: BNNSReduceFunctionSum,
                                               epsilon: 0)

let reductionLayer = BNNSFilterCreateLayerReduction(&layerParams, nil)
defer {
    BNNSFilterDestroy(reductionLayer)
}

var destinationData: [Float] = [0, 0, 0]

BNNSFilterApply(reductionLayer,
                sourceData,
                &destinationData)
```

On return, destination data contains `[12.0, 15.0, 18.0]`.

Use the following code to compute the sums of elements of each column:

```
outDescriptor.size = (3, 1, 0, 0, 0, 0, 0, 0)

var layerParams = BNNSLayerParametersReduction(i_desc: inDescriptor,
                                               o_desc: outDescriptor,
                                               w_desc: BNNSNDArrayDescriptor(),
                                               reduce_func: BNNSReduceFunctionSum,
                                               epsilon: 0)

let reductionLayer = BNNSFilterCreateLayerReduction(&layerParams, nil)
defer {
    BNNSFilterDestroy(reductionLayer)
}

var destinationData: [Float] = [0, 0, 0]

BNNSFilterApply(reductionLayer,
                sourceData,
                &destinationData)
```

On return, destination data contains `[6.0, 15.0, 24.0]`.

Use the following code to compute the sum of all elements:

```
outDescriptor.size = (1, 1, 0, 0, 0, 0, 0, 0)

var layerParams = BNNSLayerParametersReduction(i_desc: inDescriptor,
                                               o_desc: outDescriptor,
                                               w_desc: BNNSNDArrayDescriptor(),
                                               reduce_func: BNNSReduceFunctionSum,
                                               epsilon: 0)

let reductionLayer = BNNSFilterCreateLayerReduction(&layerParams, nil)
defer {
    BNNSFilterDestroy(reductionLayer)
}

var destinationData: [Float] = [0]

BNNSFilterApply(reductionLayer,
                sourceData,
                &destinationData)
```

On return, destination data contains `[45.0]`.

## See Also

### Reduction layers

class ReductionLayer

A layer object that wraps a reduction filter and manages its deinitialization.

Deprecated

static func applyReduction(BNNS.ReductionFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Applies the specified reduction function.

struct BNNSReduceFunction

Constants that describe reduction functions.

struct BNNSLayerParametersReduction

A set of parameters that define a reduction layer.

func BNNSDirectApplyReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a reduction operation directly to an input tensor.

