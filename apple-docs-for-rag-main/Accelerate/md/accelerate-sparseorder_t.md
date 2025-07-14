

- Accelerate
-  SparseOrder_t 

Structure

# SparseOrder_t

Options that define which ordering algorithm to use.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseOrder_t
```

## Overview

The column and row ordering you use when eliminating variables in a sparse factorization has a significant influence on the size of the resulting factors and the amount of work necessary to calculate them. Minimizing the size or the amount of work is an NP-complete problem, so the system only implements heuristics in this library.

Approximate minimum degree (AMD)-based orderings tend to be fast and provide good quality for small matrices. Conversely, nested dissection-based orderings, such as METIS, are usually considerably slower to compute, but provide better quality orderings for larger problems, and expose more parallelism during the factorization. Use AMD unless the problem is very large (millions of rows and columns) to avoid performing many repeated factorizations. If you’re uncertain, try both and see which gives better performance for your usage.

AMD and METIS provide good orderings for symmetric matrices. You can use them for QR factorizations, but that involves forming *AᵀA* explicitly, which is expensive. Alternatively, column AMD (COLAMD) finds an ordering for *AᵀA* while only working with *A*. For this reason, you can’t use COLAMD for symmetric factorizations.

## Topics

### Constants

var SparseOrderDefault: SparseOrder_t

The default ordering.

var SparseOrderUser: SparseOrder_t

The user-supplied ordering, or identity if the order parameter is null.

var SparseOrderAMD: SparseOrder_t

Approximate minimum degree (AMD) ordering.

var SparseOrderMetis: SparseOrder_t

METIS nested dissection ordering.

var SparseOrderCOLAMD: SparseOrder_t

The column AMD ordering for *AᵀA*.

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

### Inspecting Symbolic Factor Options

var control: SparseControl_t

The flags that control the computation.

struct SparseControl_t

Options that control the computation.

var orderMethod: SparseOrder_t

The ordering algorithm.

var order: UnsafeMutablePointer&lt;Int32>?

The user-supplied array for ordering.

var ignoreRowsAndColumns: UnsafeMutablePointer&lt;Int32>?

An array that contains row and column indices to ignore.

var malloc: (Int) -> UnsafeMutableRawPointer?

The function for allocating any necessary storage.

var free: (UnsafeMutableRawPointer?) -> Void

The function for freeing allocated storage.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

The function for reporting parameter errors.

