

- Accelerate
- SparseLSMROptions
-  conditionLimit 

Instance Property

# conditionLimit

The condition number limit (Fong-Saunders test only).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var conditionLimit: Double
```

## Discussion

The operation terminates iterations if a computed estimate of `cond(Abar)` exceeds this value. This is to prevent certain small or zero singular values of *A* or *Abar* from coming into effect and causing unwanted growth in the computed solution.

You can use conditionLimit and lambda separately or together to regularize ill-conditioned systems.

Normally, conditionLimit is in the range `1000` to `1/eps`.

Suggested value: conditionLimit `= 1/(100*eps)` for compatible systems, conditionLimit `= 1/(10*sqrt(eps))` for least squares

## See Also

### Inspecting LSMR Options

var atol: Double

The absolute tolerance (default test) or *A* tolerance (Fong-Saunders test).

var btol: Double

The *B* tolerance (Fong-Saunders test only).

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

var rtol: Double

The relative convergence tolerance (default test only).

