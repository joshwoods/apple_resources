

- Accelerate
- SparseCGOptions
-  rtol 

Instance Property

# rtol

The relative convergence tolerance.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rtol: Double
```

## Discussion

*‖ b-Ax ‖₂ \rtol is equal to `0`, the operation uses the default value of `sqrt(epsilon)`.

If it’s negative, the operation treats rtol as `0.0` (it doesn’t use the default).

## See Also

### Inspecting CG Options

var atol: Double

The absolute convergence tolerance.

var maxIterations: Int32

The maximum number of iterations to perform.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

An optional error-reporting routine.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

The function to report status.

