

- Accelerate
- SparseCGOptions
-  atol 

Instance Property

# atol

The absolute convergence tolerance.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var atol: Double
```

## Discussion

*‖ b-Ax ‖₂ \

## See Also

### Inspecting CG Options

var maxIterations: Int32

The maximum number of iterations to perform.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

An optional error-reporting routine.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

The function to report status.

var rtol: Double

The relative convergence tolerance.

