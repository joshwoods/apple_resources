

- ML Compute
- MLCSoftmaxLayer
-  init(operation:dimension:) Deprecated

Initializer

# init(operation:dimension:)

Creates a softmax layer with the operation and dimension you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    operation: MLCSoftmaxOperation,
    dimension: Int
)
```

## Parameters 

`operation`  

The softmax operation.

`dimension`  

The dimension over which you perform the softmax operation.

## See Also

### Creating Softmax Layers

convenience init(operation: MLCSoftmaxOperation)

Creates a softmax layer with the operation you specify.

Deprecated

enum MLCSoftmaxOperation

A softmax operation.

Deprecated

