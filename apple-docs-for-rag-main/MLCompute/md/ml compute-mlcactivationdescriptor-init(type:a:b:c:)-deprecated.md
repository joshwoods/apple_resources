

- ML Compute
- MLCActivationDescriptor
-  init(type:a:b:c:) Deprecated

Initializer

# init(type:a:b:c:)

Creates an activation descriptor with the activation type and parameters a, b, and c that you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    type activationType: MLCActivationType,
    a: Float,
    b: Float,
    c: Float
)
```

## Parameters 

`activationType`  

A type of activation function.

`a`  

Parameter a.

`b`  

Parameter b.

`c`  

Parameter c.

## See Also

### Creating Activation Descriptors

convenience init?(type: MLCActivationType)

Creates an activation descriptor with the activation type you specify.

Deprecated

convenience init?(type: MLCActivationType, a: Float)

Creates an activation descriptor with the activation type and parameter a that you specify.

Deprecated

convenience init?(type: MLCActivationType, a: Float, b: Float)

Creates an activation descriptor with the activation type and parameters a and b that you specify.

Deprecated

enum MLCActivationType

An activation type that you specify for an activation descriptor.

Deprecated

