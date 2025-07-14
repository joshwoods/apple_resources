

- Accelerate
- SparseGMRESOptions
-  maxIterations 

Instance Property

# maxIterations

The maximum number of iterations to perform.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var maxIterations: Int32
```

## Discussion

If `0`, the operation uses the default value of `100`.

## See Also

### Inspecting GMRES Options

var atol: Double

The absolute convergence tolerance.

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

