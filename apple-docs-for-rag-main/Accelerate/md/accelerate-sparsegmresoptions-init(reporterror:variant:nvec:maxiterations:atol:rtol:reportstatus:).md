

- Accelerate
- SparseGMRESOptions
-  init(reportError:variant:nvec:maxIterations:atol:rtol:reportStatus:) 

Initializer

# init(reportError:variant:nvec:maxIterations:atol:rtol:reportStatus:)

Returns a new GMRES options structure using the specified parameters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    reportError: ((UnsafePointer) -> Void)?,
    variant: SparseGMRESVariant_t,
    nvec: Int32,
    maxIterations: Int32,
    atol: Double,
    rtol: Double,
    reportStatus: ((UnsafePointer) -> Void)?
)
```

## Parameters 

`reportError`  

An optional error-reporting routine.

`variant`  

The exact variant of GMRES to implement.

`nvec`  

The number of orthogonal vectors the operation maintains.

`maxIterations`  

The maximum number of iterations to perform.

`atol`  

The absolute convergence tolerance.

`rtol`  

The relative convergence tolerance.

`reportStatus`  

The function to report status.

## See Also

### Initializers

init()

