

- Accelerate
-  sparse_get_vector_nonzero_count_double(\_:\_:\_:) 

Function

# sparse_get_vector_nonzero_count_double(\_:\_:\_:)

Returns the number of nonzero values in the double-precision dense vector *x*.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_get_vector_nonzero_count_double(
    _ N: sparse_dimension,
    _ x: UnsafePointer!,
    _ incx: sparse_stride
) -> Int
```

## Parameters 

`N`  

The number of elements in the dense vector *x*.

`x`  

Pointer to the vector *x*.

`incx`  

Increment between valid values in the dense vector x. Negative strides are supported.

## Return Value

The count of the nonzero values in the vector *x*.

## Discussion

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Sparse Utility Operations

func sparse_get_vector_nonzero_count_float(sparse_dimension, UnsafePointer&lt;Float>!, sparse_stride) -> Int

Returns the number of nonzero values in the single-precision dense vector *x*.

func sparse_pack_vector_double(sparse_dimension, sparse_dimension, UnsafePointer&lt;Double>!, sparse_stride, UnsafeMutablePointer&lt;Double>!, UnsafeMutablePointer&lt;sparse_index>!) -> Int

Packs nonzero values from a double-precision dense vector to a destination array.

func sparse_pack_vector_float(sparse_dimension, sparse_dimension, UnsafePointer&lt;Float>!, sparse_stride, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;sparse_index>!) -> Int

Packs nonzero values from a single-precision dense vector to a destination array.

func sparse_unpack_vector_double(sparse_dimension, sparse_dimension, Bool, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, UnsafeMutablePointer&lt;Double>!, sparse_stride)

Extracts elements from the sparse vector *x* into the corresponding location in the dense vector *y*, with both vectors containing double-precision values.

func sparse_unpack_vector_float(sparse_dimension, sparse_dimension, Bool, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!, UnsafeMutablePointer&lt;Float>!, sparse_stride)

Extracts elements from the sparse vector *x* into the corresponding location in the dense vector *y*, with both vectors containing single-precision values.

