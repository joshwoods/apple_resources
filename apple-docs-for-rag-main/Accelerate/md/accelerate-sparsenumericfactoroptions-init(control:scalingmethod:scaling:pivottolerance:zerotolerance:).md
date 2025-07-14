

- Accelerate
- SparseNumericFactorOptions
-  init(control:scalingMethod:scaling:pivotTolerance:zeroTolerance:) 

Initializer

# init(control:scalingMethod:scaling:pivotTolerance:zeroTolerance:)

Returns a new numeric factor options structure with the specified properties.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    control: SparseControl_t,
    scalingMethod: SparseScaling_t,
    scaling: UnsafeMutableRawPointer?,
    pivotTolerance: Double,
    zeroTolerance: Double
)
```

## Parameters 

`control`  

The flags that control the computation.

`scalingMethod`  

The scaling method.

`scaling`  

An array that scales the matrix before factorization.

`pivotTolerance`  

The pivot tolerance that threshold partial pivoting uses.

`zeroTolerance`  

The zero tolerance that some pivoting modes use.

## Discussion

Note

Only the symmetric factorization algorithms use the pivotTolerance and zeroTolerance parameters. SparseFactorizationQR ignores the pivot and zero tolerance values.

## See Also

### Creating a Numeric Factor Options Stucture

init()

Returns a new numeric factor options structure with default properties.

