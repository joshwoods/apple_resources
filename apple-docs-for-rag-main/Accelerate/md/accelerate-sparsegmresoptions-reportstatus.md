

- Accelerate
- SparseGMRESOptions
-  reportStatus 

Instance Property

# reportStatus

The function to report status.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var reportStatus: ((UnsafePointer) -> Void)?
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

var rtol: Double

The relative convergence tolerance.

var variant: SparseGMRESVariant_t

The exact variant of GMRES to implement.

struct SparseGMRESVariant_t

Defines the exact variant of GMRES to implement

