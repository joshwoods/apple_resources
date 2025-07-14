

- Accelerate
-  SparseNumericFactorOptions 

Structure

# SparseNumericFactorOptions

A structure that contains options that affect the numerical stage of a sparse factorization.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseNumericFactorOptions
```

## Overview

SparseNumericFactorOptions supports the following types of scaling:

| SparseScalingDefault | Default scaling — SparseScalingEquilibriationInf if *LDLᵀ*, or no scaling if Cholesky. |
|----|----|
| SparseScalingUser | User scaling if scaling is nonnull; otherwise, no scaling. |
| SparseScalingEquilibriationInf | Norm equilibration scaling using infinity norm. |

Note that the system clamps pivotTolerance to range `[0,0.5]`.

## Topics

### Creating a Numeric Factor Options Stucture

init(control: SparseControl_t, scalingMethod: SparseScaling_t, scaling: UnsafeMutableRawPointer?, pivotTolerance: Double, zeroTolerance: Double)

Returns a new numeric factor options structure with the specified properties.

init()

Returns a new numeric factor options structure with default properties.

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

var zeroTolerance: Double

The zero tolerance that some pivoting modes use.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures that Specify Factorization Type and Factorization Options

struct SparseFactorization_t

Constants that define the factorization type.

struct SparseSymbolicFactorOptions

A structure that contains options that affect the symbolic stage of a sparse factorization.

