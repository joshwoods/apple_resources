

- Accelerate
- SparseNumericFactorOptions
-  control 

Instance Property

# control

The flags that control the computation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var control: SparseControl_t
```

## See Also

### Instance Properties

struct SparseControl_t

Options that control the computation.

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

