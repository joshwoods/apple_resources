

- Accelerate
- SparseNumericFactorOptions
-  scalingMethod 

Instance Property

# scalingMethod

The scaling method.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var scalingMethod: SparseScaling_t
```

## See Also

### Instance Properties

var control: SparseControl_t

The flags that control the computation.

struct SparseControl_t

Options that control the computation.

var scaling: UnsafeMutableRawPointer?

An array that scales the matrix before factorization.

struct SparseScaling_t

Options that define which scaling algorithm to use.

var pivotTolerance: Double

The pivot tolerance that threshold partial pivoting uses.

var zeroTolerance: Double

The zero tolerance that some pivoting modes use.

