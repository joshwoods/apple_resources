

- Accelerate
-  BNNSFilterCreateLayerResize(\_:\_:) Deprecated

Function

# BNNSFilterCreateLayerResize(\_:\_:)

Returns a new resize layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterCreateLayerResize(
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

Use a resize layer to copy data between two differently sized tensors using a specified interpolation method. Resized dimensions must all either upsample or downsample; the resize layer doesn’t support combining both directions in a single operation.

For example, to resize the following source data to the specified destination dimensions:

```
let sourceData: [Float] = [0, 1, 0,
                           1, 1, 1,
                           0, 1, 0]

let destinationWidth = 24
let destinationHeight = 9

var destinationData = [Float](repeating: 0,
                              count: destinationWidth * destinationHeight)
```

Use the following code:

```

let inputDescriptor = BNNSNDArrayDescriptor(flags: flags,
                                           layout: BNNSDataLayoutRowMajorMatrix,
                                           size: (3, 3, 0, 0, 0, 0, 0, 0),
                                           stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                           data: nil,
                                           data_type: .float,
                                           table_data: nil,
                                           table_data_type: .float,
                                           data_scale: 1,
                                           data_bias: 0)

let outputDescriptor = BNNSNDArrayDescriptor(flags: flags,
                                            layout: BNNSDataLayoutRowMajorMatrix,
                                            size: (destinationWidth, destinationHeight, 0, 0, 0, 0, 0, 0),
                                            stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                            data: nil,
                                            data_type: .float,
                                            table_data: nil,
                                            table_data_type: .float,
                                            data_scale: 1,
                                            data_bias: 0)

var params = BNNSLayerParametersResize(method: BNNSInterpolationMethodNearest,
                                       i_desc: inputDescriptor,
                                       o_desc: outputDescriptor,
                                       align_corners: false)

let filter = BNNSFilterCreateLayerResize(&params, nil)

defer {
    BNNSFilterDestroy(filter)
}

BNNSFilterApply(filter,
                sourceData,
                &destinationData)
```

On return, `destinationData` contains the following values:

```
0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 0 0 0 0 0 0 0 0 
0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 0 0 0 0 0 0 0 0 
0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 0 0 0 0 0 0 0 0 
1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 
1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 
1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 
0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 0 0 0 0 0 0 0 0 
0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 0 0 0 0 0 0 0 0 
0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 0 0 0 0 0 0 0 0 
```

## See Also

### Resize layers

class ResizeLayer

A layer object that wraps a resize filter and manages its deinitialization.

Deprecated

struct BNNSInterpolationMethod

Constants that describe interpolation methods.

struct BNNSLayerParametersResize

A structure that contains the parameters of a resize layer.

Deprecated

