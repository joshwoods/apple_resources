

- Accelerate
- BNNSActivation
-  init(function:alpha:beta:) Deprecated

Initializer

# init(function:alpha:beta:)

Returns a new common activation function parameters structure that uses the specified function, alpha, and beta.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+visionOSwatchOS 3.0+tvOS 10.0+

``` source
init(
    function: BNNSActivationFunction,
    alpha: Float = .nan,
    beta: Float = .nan
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`function`  

The activation function to use.

`alpha`  

The parameter for the alpha of the activation function.

`beta`  

The parameter for the beta of the activation function.

## Return Value

A new common activation function parameters structure.

## See Also

### Initializers

init()

Returns a new common activation function parameters structure.

init(function: BNNSActivationFunction, alpha: Float, beta: Float, iscale: Int32, ioffset: Int32, ishift: Int32, iscale_per_channel: UnsafePointer&lt;Int32>?, ioffset_per_channel: UnsafePointer&lt;Int32>?, ishift_per_channel: UnsafePointer&lt;Int32>?)

Returns a new common activation function parameters structure that uses the specified function, alpha, beta, integer scale, offset, and shift.

