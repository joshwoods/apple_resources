

- Accelerate
- SparseLSMROptions
-  reportError 

Instance Property

# reportError

An optional error-reporting routine.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var reportError: ((UnsafePointer) -> Void)?
```

## See Also

### Inspecting LSMR Options

var atol: Double

The absolute tolerance (default test) or *A* tolerance (Fong-Saunders test).

var btol: Double

The *B* tolerance (Fong-Saunders test only).

var conditionLimit: Double

The condition number limit (Fong-Saunders test only).

var convergenceTest: SparseLSMRConvergenceTest_t

The convergence test to use for iterative solve methods.

struct SparseLSMRConvergenceTest_t

Constants that specify the type of convergence test.

var lambda: Double

The damping parameter lambda for regularized least squares.

var maxIterations: Int32

The maximum number of iterations.

var nvec: Int32

The number of vectors to use for local reorthogonalization.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

An optional status-reporting routine.

var rtol: Double

The relative convergence tolerance (default test only).

