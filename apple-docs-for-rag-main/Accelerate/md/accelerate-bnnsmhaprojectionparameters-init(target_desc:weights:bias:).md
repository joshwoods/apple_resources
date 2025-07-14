

- Accelerate
- BNNSMHAProjectionParameters
-  init(target_desc:weights:bias:) 

Initializer

# init(target_desc:weights:bias:)

Returns a new multihead attention projection parameters structure from the specified parameters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    target_desc: BNNSNDArrayDescriptor,
    weights: BNNSNDArrayDescriptor,
    bias: BNNSNDArrayDescriptor
)
```

## Parameters 

`target_desc`  

The descriptor—which is either an input query, key, or value, or an output—of the main target of the operation.

`weights`  

The descriptor of the initial projection’s weights.

`bias`  

The descriptor of the initial projection’s bias.

## See Also

### Initializers

init()

Returns a new multihead attention projection parameters structure.

