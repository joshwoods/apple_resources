

- Accelerate
-  sparse_inner_product_dense_float(\_:\_:\_:\_:\_:) 

Function

# sparse_inner_product_dense_float(\_:\_:\_:\_:\_:)

Computes the inner product of sparse vector *x* with dense vector *y,* with both vectors containing single-precision values.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_inner_product_dense_float(
    _ nz: sparse_dimension,
    _ x: UnsafePointer!,
    _ indx: UnsafePointer!,
    _ y: UnsafePointer!,
    _ incy: sparse_stride
) -> Float
```

## Parameters 

`nz`  

The number of nonzero entries in the sparse vector x.

`x`  

Pointer to the dense storage for the values of the sparse vector *x*. The corresponding entry in `indx` holds the index of the value. Contains `nz` values.

`indx`  

Pointer to the dense storage for the index values of the sparse vector *x*. The corresponding entry in *x* holds the values of the vector. Contains `nz` values.

`y`  

Pointer to the dense vector *y*. Accessed as `y[indx[0..nz-1]*incy]`, so dimension must be compatible with largest index value in `indx`. The behavior of this function is undefined if this is not met. Negative strides are supported. Note, unlike dense BLAS routines, the pointer points to the last element when stride is negative.

`incy`  

Increment between valid values in the dense vector y. Negative strides are supported.

## Return Value

The inner product of sparse vector *x* with dense vector *y*. Returns zero if `nz` is less than or equal to zero.

## Discussion

Indices in `indx` are always assumed to be stored in ascending order. Additionally, indices are assumed to be unique. The behavior of this function is undefined if either of these assumptions are not met.

All indices are 0 based (the first element of a pointer is `ptr[0]`).

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Vector-Vector Operations

func sparse_inner_product_dense_double(sparse_dimension, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, UnsafePointer&lt;Double>!, sparse_stride) -> Double

Computes the inner product of sparse vector *x* with double-precision *y*, with both vectors containing double-precision values.

func sparse_inner_product_sparse_double(sparse_dimension, sparse_dimension, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!) -> Double

Computes the inner product of sparse vector *x* with sparse vector *y,* with both vectors containing double-precision values.

func sparse_inner_product_sparse_float(sparse_dimension, sparse_dimension, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!) -> Float

Computes the inner product of sparse vector *x* with sparse vector *y,* with both vectors containing single-precision values.

func sparse_vector_add_with_scale_dense_double(sparse_dimension, Double, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, UnsafeMutablePointer&lt;Double>!, sparse_stride)

Scales the sparse vector *x* by *alpha* and adds the result to the dense vector *y,* with both vectors containing double-precision values.

func sparse_vector_add_with_scale_dense_float(sparse_dimension, Float, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!, UnsafeMutablePointer&lt;Float>!, sparse_stride)

Scales the sparse vector *x* by *alpha* and adds the result to the dense vector *y,* with both vectors containing single-precision values.

func sparse_vector_norm_double(sparse_dimension, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, sparse_norm) -> Double

Computes the specified norm of the double-precision sparse vector *x*.

func sparse_vector_norm_float(sparse_dimension, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!, sparse_norm) -> Float

Computes the specified norm of the single-precision sparse vector *x*.

