

- ML Compute
- MLCTransposeLayer
-  init(dimensions:) Deprecated

Initializer

# init(dimensions:)

Creates a transpose layer with the dimensions you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init?(dimensions: [Int])
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`dimensions`  

An array that represents the ordering of dimensions.

## Discussion

The `dimensions` array contains an input axis source for each output axis. In other words, the `n`th element in the dimensions array specifies the input axis source for the `n`th axis in the output. You can’t transpose the batch dimension, which is typically axis 0.

