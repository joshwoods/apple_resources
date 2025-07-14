

- Accelerate
- SparseNumericFactorOptions
-  pivotTolerance 

Instance Property

# pivotTolerance

The pivot tolerance that threshold partial pivoting uses.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var pivotTolerance: Double
```

## Discussion

The system clamps this to range `[0,0.5]`.

Note

Only the symmetric factorization algorithms use the pivotTolerance parameter. SparseFactorizationQR ignores the pivot tolerance value.

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

var zeroTolerance: Double

The zero tolerance that some pivoting modes use.

