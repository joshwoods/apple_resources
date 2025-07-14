

- Accelerate
- SparseGMRESOptions
-  reportError 

Instance Property

# reportError

An optional error-reporting routine.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var reportError: ((UnsafePointer) -> Void)?
```

## See Also

### Inspecting GMRES Options

var atol: Double

The absolute convergence tolerance.

var maxIterations: Int32

The maximum number of iterations to perform.

var nvec: Int32

The number of orthogonal vectors the operation maintains.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

The function to report status.

var rtol: Double

The relative convergence tolerance.

var variant: SparseGMRESVariant_t

The exact variant of GMRES to implement.

struct SparseGMRESVariant_t

Defines the exact variant of GMRES to implement

