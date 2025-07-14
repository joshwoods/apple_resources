

- Accelerate
- SparseCGOptions
-  init(reportError:maxIterations:atol:rtol:reportStatus:) 

Initializer

# init(reportError:maxIterations:atol:rtol:reportStatus:)

Returns a new CG options structure using the specified parameters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    reportError: ((UnsafePointer) -> Void)?,
    maxIterations: Int32,
    atol: Double,
    rtol: Double,
    reportStatus: ((UnsafePointer) -> Void)?
)
```

## Parameters 

`reportError`  

An optional error-reporting routine.

`maxIterations`  

The maximum number of iterations.

`atol`  

The absolute convergence tolerance.

`rtol`  

The relative convergence tolerance.

`reportStatus`  

The function to report status.

## Return Value

A new CG options structure.

## See Also

### Initializers

init()

Returns a new CG options structure.

