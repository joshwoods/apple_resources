

- Accelerate
- SparseLSMROptions
-  maxIterations 

Instance Property

# maxIterations

The maximum number of iterations.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var maxIterations: Int32
```

## Discussion

If maxIterations is less than `0`, the operation uses a default value of `4n`. However, if a good preconditioner is available or the matrix is well-conditioned such that singular values cluster, a value of `n/2` may be more appropriate.

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

var nvec: Int32

The number of vectors to use for local reorthogonalization.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

An optional error-reporting routine.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

An optional status-reporting routine.

var rtol: Double

The relative convergence tolerance (default test only).

