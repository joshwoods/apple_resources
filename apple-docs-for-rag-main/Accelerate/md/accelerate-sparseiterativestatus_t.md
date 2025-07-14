

- Accelerate
-  SparseIterativeStatus_t 

Structure

# SparseIterativeStatus_t

Constants that define the status of the iterative solve.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseIterativeStatus_t
```

## Topics

### Constants

var SparseIterativeConverged: SparseIterativeStatus_t

A status that indicates the convergence of all solutions.

var SparseIterativeIllConditioned: SparseIterativeStatus_t

A status that indicates the operation determines the problem is sufficiently ill-conditioned that convergence is unlikely.

var SparseIterativeInternalError: SparseIterativeStatus_t

A status that indicates an internal failure.

var SparseIterativeMaxIterations: SparseIterativeStatus_t

A status that indicates a failure to converge one or more solutions in the maximum number of iterations.

var SparseIterativeParameterError: SparseIterativeStatus_t

A status that indicates an error with one or more parameters.

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

