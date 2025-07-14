

- Accelerate
-  SparseGMRESVariant_t 

Structure

# SparseGMRESVariant_t

Defines the exact variant of GMRES to implement

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseGMRESVariant_t
```

## Topics

### Constants

var SparseVariantDQGMRES: SparseGMRESVariant_t

A constant that specifies the DQGMRES variant.

var SparseVariantFGMRES: SparseGMRESVariant_t

A constant that specifies the flexible GMRES variant.

var SparseVariantGMRES: SparseGMRESVariant_t

A constant that specifies the standard restarted GMRES variant.

### Raw Values

init(UInt8)

init(rawValue: UInt8)

var rawValue: UInt8

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting GMRES Options

var atol: Double

The absolute convergence tolerance.

var maxIterations: Int32

The maximum number of iterations to perform.

var nvec: Int32

The number of orthogonal vectors the operation maintains.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

An optional error-reporting routine.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

The function to report status.

var rtol: Double

The relative convergence tolerance.

var variant: SparseGMRESVariant_t

The exact variant of GMRES to implement.

