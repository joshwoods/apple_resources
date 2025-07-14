

- Accelerate
-  sparse_norm 

Structure

# sparse_norm

The norm specifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct sparse_norm
```

## Overview

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## Topics

### Constants

var SPARSE_NORM_ONE: sparse_norm

Norm One

var SPARSE_NORM_TWO: sparse_norm

Norm Two

var SPARSE_NORM_INF: sparse_norm

Norm Inf

var SPARSE_NORM_R1: sparse_norm

Norm R1

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting Types

typealias sparse_matrix_double

Sparse matrix opaque type for double.

typealias sparse_matrix_float

Sparse matrix opaque type for float.

struct sparse_status

The type reflecting the status of an operations.

typealias sparse_dimension

The dimension type.

typealias sparse_index

The index type.

typealias sparse_stride

The stride type.

