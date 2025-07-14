

- Accelerate
-  sparse_status 

Structure

# sparse_status

The type reflecting the status of an operations.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct sparse_status
```

## Overview

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## Topics

### Constants

var SPARSE_SUCCESS: sparse_status

Operation was a success.

var SPARSE_ILLEGAL_PARAMETER: sparse_status

Operation was not completed because one or more of the arguments had an illegal value.

var SPARSE_CANNOT_SET_PROPERTY: sparse_status

A property was set after values were inserted into the matrix.

var SPARSE_SYSTEM_ERROR: sparse_status

An internal error has occured, such as non enough memory.

### Initializers

init(Int32)

init(rawValue: Int32)

### Instance Properties

var rawValue: Int32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting Types

typealias sparse_dimension

The dimension type.

typealias sparse_index

The index type.

typealias sparse_matrix_double

Sparse matrix opaque type for double.

typealias sparse_matrix_float

Sparse matrix opaque type for float.

