

- Accelerate
-  SparseSymbolicFactorOptions 

Structure

# SparseSymbolicFactorOptions

A structure that contains options that affect the symbolic stage of a sparse factorization.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseSymbolicFactorOptions
```

## Mentioned in 

Solving systems using direct methods

## Overview

SparseSymbolicFactorOptions supports the following ordering algorithms:

| SparseOrderDefault | The default ordering (SparseOrderAMD for symmetric and SparseOrderCOLAMD for unsymmetric factorizations). |
|----|----|
| SparseOrderUser | The user-supplied ordering, or identity if order is `null`. |
| SparseOrderAMD | Approximate minimum degree (AMD) ordering. There’s a large overhead cost if you use it for QR-based factorization due to explicit formation of *AᵀA*. |
| SparseOrderMetis | METIS nested dissection ordering. There’s a large overhead cost if you use it for QR-based factorization due to explicit formation of *AᵀA*. |
| SparseOrderCOLAMD | The column AMD ordering for *AᵀA*. This isn’t valid for symmetric factorizations (use SparseOrderAMD instead). |

## Topics

### Creating a Symbolic Factor Options Structure

init(control: SparseControl_t, orderMethod: SparseOrder_t, order: UnsafeMutablePointer&lt;Int32>?, ignoreRowsAndColumns: UnsafeMutablePointer&lt;Int32>?, malloc: (Int) -> UnsafeMutableRawPointer?, free: (UnsafeMutableRawPointer?) -> Void, reportError: ((UnsafePointer&lt;CChar>) -> Void)?)

Creates a new structure that contains options that affect the symbolic stage of a sparse factorization.

### Inspecting Symbolic Factor Options

var control: SparseControl_t

The flags that control the computation.

struct SparseControl_t

Options that control the computation.

var orderMethod: SparseOrder_t

The ordering algorithm.

var order: UnsafeMutablePointer&lt;Int32>?

The user-supplied array for ordering.

struct SparseOrder_t

Options that define which ordering algorithm to use.

var ignoreRowsAndColumns: UnsafeMutablePointer&lt;Int32>?

An array that contains row and column indices to ignore.

var malloc: (Int) -> UnsafeMutableRawPointer?

The function for allocating any necessary storage.

var free: (UnsafeMutableRawPointer?) -> Void

The function for freeing allocated storage.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

The function for reporting parameter errors.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Related Documentation

struct SparseOrder_t

Options that define which ordering algorithm to use.

### Structures that Specify Factorization Type and Factorization Options

struct SparseFactorization_t

Constants that define the factorization type.

struct SparseNumericFactorOptions

A structure that contains options that affect the numerical stage of a sparse factorization.

