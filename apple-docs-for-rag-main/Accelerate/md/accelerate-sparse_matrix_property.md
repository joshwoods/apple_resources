

- Accelerate
-  sparse_matrix_property 

Structure

# sparse_matrix_property

The matrix property type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct sparse_matrix_property
```

## Overview

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## Topics

### Constants

var SPARSE_UPPER_TRIANGULAR: sparse_matrix_property

An upper triangular matrix.

var SPARSE_LOWER_TRIANGULAR: sparse_matrix_property

A lower triangular matrix.

var SPARSE_UPPER_SYMMETRIC: sparse_matrix_property

A symmetric matrix with values derived from the upper triangle.

var SPARSE_LOWER_SYMMETRIC: sparse_matrix_property

A symmetric matrix with values derived from the lower triangle.

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

typealias sparse_dimension

The dimension type.

typealias sparse_index

The index type.

