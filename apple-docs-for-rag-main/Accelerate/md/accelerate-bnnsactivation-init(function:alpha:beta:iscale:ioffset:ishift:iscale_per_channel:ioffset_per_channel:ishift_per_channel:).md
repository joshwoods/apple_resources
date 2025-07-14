

- Accelerate
- BNNSActivation
-  init(function:alpha:beta:iscale:ioffset:ishift:iscale_per_channel:ioffset_per_channel:ishift_per_channel:) 

Initializer

# init(function:alpha:beta:iscale:ioffset:ishift:iscale_per_channel:ioffset_per_channel:ishift_per_channel:)

Returns a new common activation function parameters structure that uses the specified function, alpha, beta, integer scale, offset, and shift.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    function: BNNSActivationFunction,
    alpha: Float,
    beta: Float,
    iscale: Int32,
    ioffset: Int32,
    ishift: Int32,
    iscale_per_channel: UnsafePointer?,
    ioffset_per_channel: UnsafePointer?,
    ishift_per_channel: UnsafePointer?
)
```

## Parameters 

`function`  

The activation function.

`alpha`  

The parameter for the alpha of the activation function.

`beta`  

The parameter for the beta of the activation function.

`iscale`  

Scale for integer functions.

`ioffset`  

Offset for integer functions.

`ishift`  

Shift for integer functions.

`iscale_per_channel`  

Scale per channel for integer functions.

`ioffset_per_channel`  

Offset per channel for integer functions.

`ishift_per_channel`  

Shift per channel for integer functions.

## Return Value

A new common activation function parameters structure.

## See Also

### Initializers

init()

Returns a new common activation function parameters structure.

init(function: BNNSActivationFunction, alpha: Float, beta: Float)

Returns a new common activation function parameters structure that uses the specified function, alpha, and beta.

Deprecated

