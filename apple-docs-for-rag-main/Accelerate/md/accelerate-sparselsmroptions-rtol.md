

- Accelerate
- SparseLSMROptions
-  rtol 

Instance Property

# rtol

The relative convergence tolerance (default test only).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rtol: Double
```

## Discussion

If this value is `0.0`, the operation uses the default value of `sqrt(epsilon)`. If it’s negative, the operation treats rtol as `0.0` (it doesn’t use the default)

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

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

An optional error-reporting routine.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

An optional status-reporting routine.

