

- Accelerate
-  SparseControl_t 

Structure

# SparseControl_t

Options that control the computation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseControl_t
```

## Topics

### Constants

var SparseDefaultControl: SparseControl_t

A flag that indicates default values.

### Raw Values

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

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

var scalingMethod: SparseScaling_t

The scaling method.

var scaling: UnsafeMutableRawPointer?

An array that scales the matrix before factorization.

struct SparseScaling_t

Options that define which scaling algorithm to use.

var pivotTolerance: Double

The pivot tolerance that threshold partial pivoting uses.

var zeroTolerance: Double

The zero tolerance that some pivoting modes use.

