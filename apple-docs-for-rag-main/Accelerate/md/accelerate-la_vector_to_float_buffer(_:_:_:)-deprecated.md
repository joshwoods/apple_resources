

- Accelerate
-  la_vector_to_float_buffer(\_:\_:\_:) Deprecated

Function

# la_vector_to_float_buffer(\_:\_:\_:)

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.10–11.0DeprecatedtvOS 8.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–7.0Deprecated

``` source
func la_vector_to_float_buffer(
    _ buffer: UnsafeMutablePointer,
    _ buffer_stride: la_index_t,
    _ vector: la_object_t
) -> la_status_t
```

Deprecated

This API is deprecated, please use BLAS and LAPACK

## Parameters 

`buffer`  

Pointer to the destination buffer.

`buffer_stride`  

Offset (in floats) between the destinations of consecutive vector elements in the buffer. Negative strides are not supported (you can get the same effect by reversing the vector before calling this function).

`vector`  

The vector to store.

## Discussion

Stores the elements of a vector to a buffer.

The buffer must be large enough to accomodate the vector being stored. Specifically, it must have have sufficient space to hold

buffer_stride\*(la_vector_length(vector)-1) + 1

float elements. Real usage in the most common case (stride = 1) will look roughly like this:

la_count_t length = la_vector_length(vector); if (!length) { // an error occured. } float \*buffer = malloc(length \* sizeof buffer\[0\]); la_vector_to_float_buffer(buffer, 1, vector);

This function supports storing the contents of a vector, or a matrix that has only one row or only one column. If the object satisfies those requirements, and it does not have an error status, its contents are stored to the buffer. If it has an error status, NaNs are stored to the buffer.

If the object is not a matrix or vector, or if it is a matrix with both dimensions larger than one, nothing is written to the buffer and LA_INVALID_PARAMETER_ERROR is returned.

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

