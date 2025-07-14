

- Accelerate
- SparseGMRESOptions
-  variant 

Instance Property

# variant

The exact variant of GMRES to implement.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var variant: SparseGMRESVariant_t
```

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

var rtol: Double

The relative convergence tolerance.

struct SparseGMRESVariant_t

Defines the exact variant of GMRES to implement

