

- Accelerate
- SparseLSMROptions
-  btol 

Instance Property

# btol

The *B* tolerance (Fong-Saunders test only).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var btol: Double
```

## Discussion

This value holds an estimate of the relative error in the data defining the right-hand-side, *b*. For example, if *b* is accurate to about six digits, set btol `= 1.0e-6`.

## See Also

### Inspecting LSMR Options

var atol: Double

The absolute tolerance (default test) or *A* tolerance (Fong-Saunders test).

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

var rtol: Double

The relative convergence tolerance (default test only).

