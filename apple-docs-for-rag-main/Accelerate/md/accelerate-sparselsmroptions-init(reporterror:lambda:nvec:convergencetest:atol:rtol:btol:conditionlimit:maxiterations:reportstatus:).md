

- Accelerate
- SparseLSMROptions
-  init(reportError:lambda:nvec:convergenceTest:atol:rtol:btol:conditionLimit:maxIterations:reportStatus:) 

Initializer

# init(reportError:lambda:nvec:convergenceTest:atol:rtol:btol:conditionLimit:maxIterations:reportStatus:)

Returns a new LSMR options structure using the specified parameters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    reportError: ((UnsafePointer) -> Void)?,
    lambda: Double,
    nvec: Int32,
    convergenceTest: SparseLSMRConvergenceTest_t,
    atol: Double,
    rtol: Double,
    btol: Double,
    conditionLimit: Double,
    maxIterations: Int32,
    reportStatus: ((UnsafePointer) -> Void)?
)
```

## Parameters 

`reportError`  

An optional status-reporting routine.

`lambda`  

The damping parameter lambda for regularized least squares.

`nvec`  

The number of vectors to use for local reorthogonalization.

`convergenceTest`  

The convergence test to use for iterative solve methods.

`atol`  

The absolute tolerance (default test) or *A* tolerance (Fong-Saunders test).

`rtol`  

The relative convergence tolerance (default test only).

`btol`  

The *B* tolerance (Fong-Saunders test only).

`conditionLimit`  

The condition number limit (Fong-Saunders test only).

`maxIterations`  

The maximum number of iterations.

`reportStatus`  

An optional error-reporting routine.

## See Also

### Initializers

init()

Returns a new LSMR options structure.

