

- Accelerate
- SparseNumericFactorOptions
-  zeroTolerance 

Instance Property

# zeroTolerance

The zero tolerance that some pivoting modes use.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var zeroTolerance: Double
```

## Discussion

Note

Only the symmetric factorization algorithms use the zeroTolerance parameter. SparseFactorizationQR ignores the zero tolerance value.

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

struct SparseScaling_t

Options that define which scaling algorithm to use.

var pivotTolerance: Double

The pivot tolerance that threshold partial pivoting uses.

