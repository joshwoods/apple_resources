

- Accelerate
- SparseNumericFactorOptions
-  scaling 

Instance Property

# scaling

An array that scales the matrix before factorization.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var scaling: UnsafeMutableRawPointer?
```

## Discussion

This array can either be `nil` or a pointer to an array of real values with a length greater than or equal to the size of the matrix that you’re factoring. The type of the array values is the element type of the matrix (but real, even if the matrix is complex).

If scalingMethod is SparseScalingUser, and this pointer is `nil`, the system doesn’t apply scaling.

If scalingMethod is SparseScalingUser, and this pointer isn’t `nil`, the system uses the user-provided array to scale the matrix before factorization.

If scalingMethod isn’t SparseScalingUser, the factor function computes its own scaling.

If this pointer isn’t `nil`, the computed scaling returns in the array.

## See Also

### Instance Properties

var control: SparseControl_t

The flags that control the computation.

struct SparseControl_t

Options that control the computation.

var scalingMethod: SparseScaling_t

The scaling method.

struct SparseScaling_t

Options that define which scaling algorithm to use.

var pivotTolerance: Double

The pivot tolerance that threshold partial pivoting uses.

var zeroTolerance: Double

The zero tolerance that some pivoting modes use.

