

- Accelerate
-  BNNSFilterCreateLayerDropout(\_:\_:) Deprecated

Function

# BNNSFilterCreateLayerDropout(\_:\_:)

Returns a new dropout layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterCreateLayerDropout(
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

Use a dropout layer to randomly set the elements—or entire dimensions—of a tensor to 0. The layer scales the unchanged elements by `1 / (1 -` rate `)`. The following code randomly drops half the elements from a 4 x 4 matrix:

```
let input: [Float] = [1, 1, 1, 1,
                      1, 1, 1, 1,
                      1, 1, 1, 1,
                      1, 1, 1, 1]

var output = [Float](repeating: 0,
                     count: input.count)

let descriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                       layout: BNNSDataLayoutRowMajorMatrix,
                                       size: (4, 4, 0, 0, 0, 0, 0, 0),
                                       stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                       data: nil,
                                       data_type: .float,
                                       table_data: nil,
                                       table_data_type: .float,
                                       data_scale: 0,
                                       data_bias: 0)

let control: UInt8 = 0b0000
let rate: Float = 0.5

var dropoutParams = BNNSLayerParametersDropout(i_desc: descriptor,
                                               o_desc: descriptor,
                                               rate: rate,
                                               seed: 0,
                                               control: control)

let dropoutFilter = BNNSFilterCreateLayerDropout(&dropoutParams, nil)

BNNSFilterApply(dropoutFilter, input, &output)
```

On return, output contains the following values:

```
[ 2.0, 2.0, 0.0, 0.0, 
  2.0, 2.0, 0.0, 2.0, 
  2.0, 0.0, 0.0, 2.0, 
  0.0, 0.0, 0.0, 2.0 ]
```

Use the control parameter to dropout entire dimensions. For example, setting `control` to `0b0010` and `rate` to `0.75` drops three quarters of the columns, and scales the remaining values by 4:

```
[ 0.0, 4.0, 0.0, 0.0, 
  0.0, 4.0, 0.0, 0.0, 
  0.0, 4.0, 0.0, 0.0, 
  0.0, 4.0, 0.0, 0.0 ]
```

## See Also

### Dropout layers

class DropoutLayer

A layer object that wraps a dropout filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersDropout

A structure that contains the parameters of a dropout layer.

Deprecated

