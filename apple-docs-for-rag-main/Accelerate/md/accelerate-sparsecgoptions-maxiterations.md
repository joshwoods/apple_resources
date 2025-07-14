

- Accelerate
- SparseCGOptions
-  maxIterations 

Instance Property

# maxIterations

The maximum number of iterations to perform.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var maxIterations: Int32
```

## Discussion

If `0`, the operation uses the default value of `100`.

## See Also

### Inspecting CG Options

var atol: Double

The absolute convergence tolerance.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

An optional error-reporting routine.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

The function to report status.

var rtol: Double

The relative convergence tolerance.

