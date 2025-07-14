

- Accelerate
- SparseLSMROptions
-  convergenceTest 

Instance Property

# convergenceTest

The convergence test to use for iterative solve methods.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var convergenceTest: SparseLSMRConvergenceTest_t
```

## Discussion

For SparseLSMRCTDefault, iterations stop when:

- *‖ Aᵀ(b-Ax) ‖₂ \rtol \* ‖ Aᵀ(b-Ax_₀) ‖₂ + atol*

For SparseLSMRCTFongSaunders, iterations stop when any of the following occur:

- *‖ b-Ax ‖₂ \btol \* ‖ b ‖₂ + atol \* ‖ A ‖₂ ‖ x ‖₂* (*‖A‖₂* is an estimate)

- *‖ Aᵀ (b-Ax) ‖₂ \atol \* ‖ A ‖₂ \* ‖ A-bx ‖₂* (*‖A‖₂* is an estimate)

- Estimated condition of *matrix \>= conditionLimit*

## See Also

### Inspecting LSMR Options

var atol: Double

The absolute tolerance (default test) or *A* tolerance (Fong-Saunders test).

var btol: Double

The *B* tolerance (Fong-Saunders test only).

var conditionLimit: Double

The condition number limit (Fong-Saunders test only).

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

