

- Accelerate
-  SparseScaling_t 

Structure

# SparseScaling_t

Options that define which scaling algorithm to use.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseScaling_t
```

## Topics

### Constants

var SparseScalingDefault: SparseScaling_t

Default scaling.

var SparseScalingUser: SparseScaling_t

User scaling.

var SparseScalingEquilibriationInf: SparseScaling_t

The norm equilibration scaling using infinity norm.

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

### Instance Properties

var control: SparseControl_t

The flags that control the computation.

struct SparseControl_t

Options that control the computation.

var scalingMethod: SparseScaling_t

The scaling method.

var scaling: UnsafeMutableRawPointer?

An array that scales the matrix before factorization.

var pivotTolerance: Double

The pivot tolerance that threshold partial pivoting uses.

var zeroTolerance: Double

The zero tolerance that some pivoting modes use.

