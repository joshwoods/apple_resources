

- Accelerate
-  BNNSFilterCreateLayerPermute(\_:\_:) Deprecated

Function

# BNNSFilterCreateLayerPermute(\_:\_:)

Returns a new permute layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterCreateLayerPermute(
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

Use a permute layer to copy one tensor to another while permuting the order of the axes. For example, given a BNNSDataLayoutImageCHW tensor containing the following values:

```
let sourceData: [Int8] = [ 1,  2,
                           3,  4] +
                         [10, 20,
                          30, 40]
```

The following code copies the data from `sourceData` to `destinationData`, but with the axis order permuted from \[0, 1, 2\] to \[2, 1, 0\]:

```
var destinationData = [Int8](repeating: 0,
                              count: sourceData.count)

let descriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                       layout: BNNSDataLayoutImageCHW,
                                       size: (2, 2, 2, 0, 0, 0, 0, 0),
                                       stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                       data: nil,
                                       data_type: .int8,
                                       table_data: nil,
                                       table_data_type: .int8,
                                       data_scale: 1,
                                       data_bias: 0)

var params = BNNSLayerParametersPermute(i_desc: descriptor,
                                        o_desc: descriptor,
                                        permutation: (2, 1, 0, 0, 0, 0, 0, 0))

let filter = BNNSFilterCreateLayerPermute(&params, nil)

defer {
    BNNSFilterDestroy(filter)
}

BNNSFilterApply(filter,
                sourceData,
                &destinationData)

```

On return, `destinationData` contains `[1, 10, 3, 30, 2, 20, 4, 40]`.

The following figure shows the source data on the left, and the permute result on the right:

## See Also

### Permute layers

class PermuteLayer

A layer object that wraps a permute filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersPermute

A structure that contains the parameters of a permute layer.

Deprecated

func BNNSPermuteFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int) -> Int32

Applies a permute filter backward to generate gradients.

Deprecated

