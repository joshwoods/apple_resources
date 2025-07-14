

- Accelerate
- SparseGMRESOptions
-  atol 

Instance Property

# atol

The absolute convergence tolerance.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var atol: Double
```

## Discussion

*‖ b-Ax ‖₂ \rtol \* ‖ b-Ax₀ ‖₂ + atol* indicates convergence.

## See Also

### Inspecting GMRES Options

var maxIterations: Int32

The maximum number of iterations to perform.

var nvec: Int32

The number of orthogonal vectors the operation maintains.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

An optional error-reporting routine.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

The function to report status.

var rtol: Double

The relative convergence tolerance.

var variant: SparseGMRESVariant_t

The exact variant of GMRES to implement.

struct SparseGMRESVariant_t

Defines the exact variant of GMRES to implement

