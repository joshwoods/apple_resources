

- Accelerate
-  SparseLSMRConvergenceTest_t 

Structure

# SparseLSMRConvergenceTest_t

Constants that specify the type of convergence test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseLSMRConvergenceTest_t
```

## Topics

### Constants

var SparseLSMRCTDefault: SparseLSMRConvergenceTest_t

The default convergence test.

var SparseLSMRCTFongSaunders: SparseLSMRConvergenceTest_t

Fong and Saunder’s original convergence test.

### Raw Values

init(Int32)

init(rawValue: Int32)

var rawValue: Int32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

