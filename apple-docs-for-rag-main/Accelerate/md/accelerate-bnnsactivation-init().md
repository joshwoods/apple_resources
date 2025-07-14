

- Accelerate
- BNNSActivation
-  init() 

Initializer

# init()

Returns a new common activation function parameters structure.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init()
```

## See Also

### Initializers

init(function: BNNSActivationFunction, alpha: Float, beta: Float)

Returns a new common activation function parameters structure that uses the specified function, alpha, and beta.

Deprecated

init(function: BNNSActivationFunction, alpha: Float, beta: Float, iscale: Int32, ioffset: Int32, ishift: Int32, iscale_per_channel: UnsafePointer&lt;Int32>?, ioffset_per_channel: UnsafePointer&lt;Int32>?, ishift_per_channel: UnsafePointer&lt;Int32>?)

Returns a new common activation function parameters structure that uses the specified function, alpha, beta, integer scale, offset, and shift.

