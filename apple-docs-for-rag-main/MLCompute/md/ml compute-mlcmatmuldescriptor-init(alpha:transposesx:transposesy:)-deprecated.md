

- ML Compute
- MLCMatMulDescriptor
-  init(alpha:transposesX:transposesY:) Deprecated

Initializer

# init(alpha:transposesX:transposesY:)

Creates a batched matrix multiplication descriptor with the alpha value and transpose options you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    alpha: Float,
    transposesX: Bool,
    transposesY: Bool
)
```

## Parameters 

`alpha`  

A scalar value you specify to scale the left-hand side, `C = alpha x A x B`.

`transposesX`  

A Boolean that specifies whether you choose to transpose the last two dimensions of x.

`transposesY`  

A Boolean that specifies whether you choose to transpose the last two dimensions of y.

## See Also

### Creating Matrix Multiplication Descriptors

convenience init()

Creates a batched matrix multiplication descriptor.

Deprecated

