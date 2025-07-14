

- Accelerate
- SparseGMRESOptions
-  rtol 

Instance Property

# rtol

The relative convergence tolerance.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rtol: Double
```

## Discussion

*‖ b-Ax ‖₂ \rtol \* ‖ b-Ax₀ ‖₂ + atol* indicates convergence.

If rtol `= 0`, the operation uses the default value of `sqrt(epsilon)`.

If it’s negative, the system treats rtol as `0.0` (it doesn’t use the default).

## See Also

### Inspecting GMRES Options

var atol: Double

The absolute convergence tolerance.

var maxIterations: Int32

The maximum number of iterations to perform.

var nvec: Int32

The number of orthogonal vectors the operation maintains.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

An optional error-reporting routine.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

The function to report status.

var variant: SparseGMRESVariant_t

The exact variant of GMRES to implement.

struct SparseGMRESVariant_t

Defines the exact variant of GMRES to implement

