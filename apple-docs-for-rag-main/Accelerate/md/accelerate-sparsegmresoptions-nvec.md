

- Accelerate
- SparseGMRESOptions
-  nvec 

Instance Property

# nvec

The number of orthogonal vectors the operation maintains.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var nvec: Int32
```

## Discussion

For GMRES and FGMRES variants, this is the number of iterations between restarts. For DQGMRES it’s the number of historical vectors the operation maintains in memory. If nvec is less than or equal to `0`, the operation uses the default value of `16`.

## See Also

### Inspecting GMRES Options

var atol: Double

The absolute convergence tolerance.

var maxIterations: Int32

The maximum number of iterations to perform.

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

