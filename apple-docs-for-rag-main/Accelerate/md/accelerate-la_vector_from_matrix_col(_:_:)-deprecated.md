

- Accelerate
-  la_vector_from_matrix_col(\_:\_:) Deprecated

Function

# la_vector_from_matrix_col(\_:\_:)

Creates a vector from the specified column of the matrix.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.10–11.0DeprecatedtvOS 8.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–7.0Deprecated

``` source
func la_vector_from_matrix_col(
    _ matrix: la_object_t,
    _ matrix_col: la_count_t
) -> la_object_t
```

Deprecated

This API is deprecated, please use BLAS and LAPACK

## Parameters 

`matrix`  

Matrix from which to create the column vector.

`matrix_col`  

The zero-based index of the column to create the vector from.

## Return Value

The resulting vector is a rows(matrix) x 1 vector.

## Discussion

Creates a vector from the specified column of the matrix. If the value for `matrix_col` is less than zero or greater than `cols(matrix)-1`, `LA_INVALID_PARAMETER_ERROR` is returned.

If matrix is a splat, `LA_INVALID_PARAMETER_ERROR` is returned.

Always returns a `vector_length x 1` vector.

## See Also

### Functions

func caxpy_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ccopy_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cdotc_(OpaquePointer, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cdotu_(OpaquePointer, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cgbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cgemm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cgemv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cgerc_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cgeru_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func chbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func chemm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func chemv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cher2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cher2k_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cher_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

