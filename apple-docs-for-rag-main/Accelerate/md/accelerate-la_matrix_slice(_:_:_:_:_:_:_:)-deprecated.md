

- Accelerate
-  la_matrix_slice(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# la_matrix_slice(\_:\_:\_:\_:\_:\_:\_:)

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.10–11.0DeprecatedtvOS 8.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–7.0Deprecated

``` source
func la_matrix_slice(
    _ matrix: la_object_t,
    _ matrix_first_row: la_index_t,
    _ matrix_first_col: la_index_t,
    _ matrix_row_stride: la_index_t,
    _ matrix_col_stride: la_index_t,
    _ slice_rows: la_count_t,
    _ slice_cols: la_count_t
) -> la_object_t
```

Deprecated

This API is deprecated, please use BLAS and LAPACK

## Parameters 

`matrix`  

The matrix to be sliced.

`matrix_first_row`  

The index of the row of the source matrix containing the first element of new slice matrix.

`matrix_first_col`  

The index of the column of the source matrix containing the first element of the slice matrix.

`matrix_row_stride`  

The offset in the source matrix between rows that will be consecutive in the slice matrix.

`matrix_col_stride`  

The offset in the source matrix between columns that will be consecutve in the slice matrix.

`slice_rows`  

The number of rows in the slice matrix.

`slice_cols`  

The number of columns in the slice matrix.

## Return Value

A new matrix with size slice_rows x slice_cols whose elements are taken from the source matrix.

## Discussion

Create a slice of a matrix.

The result object is the slice_rows x slice_cols matrix whose i,jth entry is:

```
matrix[matrix_first_row + i*matrix_row_stride,
       matrix_first_col + j*matrix_col_stride]
```

Slices provide an efficient means to operate on tiles and strides. These are lightweight objects that reference the storage of the matrix from which they originate. In most cases, creating a slice does not require any allocation beyond the object representing the slice, nor require copying. In some less common cases, a copy may be required.

This function supports slicing a vector (interpreted as rows(matrix) x cols(matrix)) or a matrix. If the object is not a matrix or vector, the returned object will have status LA_INVALID_PARAMETER_ERROR.

If the slice references indices that are less than zero or greater than or equal to the dimensions of the matrix, LA_SLICE_OUT_OF_BOUNDS_ERROR is returned.

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

