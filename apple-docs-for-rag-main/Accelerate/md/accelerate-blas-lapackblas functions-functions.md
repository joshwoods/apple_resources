

- Accelerate
- BLAS
-  LAPACK/BLAS Functions 

API Collection

# LAPACK/BLAS Functions

An updated BLAS interface supporting ILP64 is available.

## Overview

Note

An updated BLAS interface supporting ILP64 is available. Please compile with -DACCELERATE_NEW_LAPACK to access the new headers and -DACCELERATE_LAPACK_ILP64 for ILP64 support.

## Topics

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

func cherk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func chpmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func chpr2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func chpr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func crotg_(OpaquePointer, OpaquePointer, UnsafeMutablePointer&lt;Float>, OpaquePointer)

func cscal_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func csrot_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>)

func csscal_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cswap_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func csymm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func csyr2k_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func csyrk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ctbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ctbsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ctpmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ctpsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ctrmm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ctrmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ctrsm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ctrsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func dasum_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>) -> Double

func daxpy_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dcopy_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func ddot_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>) -> Double

func dgbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dgemm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dgemv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dger_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dnrm2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>) -> Double

func drot_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>)

func drotg_(UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func drotm_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>)

func drotmg_(UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dsbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dscal_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dsdot_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>) -> Double

func dspmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dspr2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func dspr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func dswap_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dsymm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dsymv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dsyr2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dsyr2k_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dsyr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dsyrk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dtbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dtbsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dtpmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dtpsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dtrmm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dtrmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dtrsm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dtrsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dzasum_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> Double

func dznrm2_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> Double

func icamax_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func idamax_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func isamax_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func izamax_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func la_add_attributes(la_object_t, la_attribute_t)Deprecated

func la_diagonal_matrix_from_vector(la_object_t, la_index_t) -> la_object_tDeprecated

func la_difference(la_object_t, la_object_t) -> la_object_tDeprecated

func la_elementwise_product(la_object_t, la_object_t) -> la_object_tDeprecated

func la_identity_matrix(la_count_t, la_scalar_type_t, la_attribute_t) -> la_object_tDeprecated

func la_inner_product(la_object_t, la_object_t) -> la_object_tDeprecated

func la_matrix_cols(la_object_t) -> la_count_tDeprecated

func la_matrix_from_double_buffer(UnsafePointer&lt;Double>, la_count_t, la_count_t, la_count_t, la_hint_t, la_attribute_t) -> la_object_tDeprecated

func la_matrix_from_double_buffer_nocopy(UnsafeMutablePointer&lt;Double>, la_count_t, la_count_t, la_count_t, la_hint_t, la_deallocator_t?, la_attribute_t) -> la_object_tDeprecated

func la_matrix_from_float_buffer(UnsafePointer&lt;Float>, la_count_t, la_count_t, la_count_t, la_hint_t, la_attribute_t) -> la_object_tDeprecated

func la_matrix_from_float_buffer_nocopy(UnsafeMutablePointer&lt;Float>, la_count_t, la_count_t, la_count_t, la_hint_t, la_deallocator_t?, la_attribute_t) -> la_object_tDeprecated

func la_matrix_from_splat(la_object_t, la_count_t, la_count_t) -> la_object_tDeprecated

func la_matrix_product(la_object_t, la_object_t) -> la_object_tDeprecated

func la_matrix_rows(la_object_t) -> la_count_tDeprecated

func la_matrix_slice(la_object_t, la_index_t, la_index_t, la_index_t, la_index_t, la_count_t, la_count_t) -> la_object_tDeprecated

func la_matrix_to_double_buffer(UnsafeMutablePointer&lt;Double>, la_count_t, la_object_t) -> la_status_tDeprecated

func la_matrix_to_float_buffer(UnsafeMutablePointer&lt;Float>, la_count_t, la_object_t) -> la_status_tDeprecated

func la_norm_as_double(la_object_t, la_norm_t) -> DoubleDeprecated

func la_norm_as_float(la_object_t, la_norm_t) -> FloatDeprecated

func la_normalized_vector(la_object_t, la_norm_t) -> la_object_tDeprecated

func la_outer_product(la_object_t, la_object_t) -> la_object_tDeprecated

func la_release(la_object_t)Deprecated

func la_remove_attributes(la_object_t, la_attribute_t)Deprecated

func la_retain(la_object_t) -> la_object_tDeprecated

func la_scale_with_double(la_object_t, Double) -> la_object_tDeprecated

func la_scale_with_float(la_object_t, Float) -> la_object_tDeprecated

func la_solve(la_object_t, la_object_t) -> la_object_tDeprecated

func la_splat_from_double(Double, la_attribute_t) -> la_object_tDeprecated

func la_splat_from_float(Float, la_attribute_t) -> la_object_tDeprecated

func la_splat_from_matrix_element(la_object_t, la_index_t, la_index_t) -> la_object_tDeprecated

func la_splat_from_vector_element(la_object_t, la_index_t) -> la_object_tDeprecated

func la_status(la_object_t) -> la_status_tDeprecated

func la_sum(la_object_t, la_object_t) -> la_object_tDeprecated

func la_transpose(la_object_t) -> la_object_tDeprecated

func la_vector_from_matrix_col(la_object_t, la_count_t) -> la_object_t

Creates a vector from the specified column of the matrix.

Deprecated

func la_vector_from_matrix_diagonal(la_object_t, la_index_t) -> la_object_t

Creates a vector from the specified diagonal of the matrix.

Deprecated

func la_vector_from_matrix_row(la_object_t, la_count_t) -> la_object_t

Creates a vector from the specified row of the matrix.

Deprecated

func la_vector_from_splat(la_object_t, la_count_t) -> la_object_tDeprecated

func la_vector_length(la_object_t) -> la_count_tDeprecated

func la_vector_slice(la_object_t, la_index_t, la_index_t, la_count_t) -> la_object_tDeprecated

func la_vector_to_double_buffer(UnsafeMutablePointer&lt;Double>, la_index_t, la_object_t) -> la_status_tDeprecated

func la_vector_to_float_buffer(UnsafeMutablePointer&lt;Float>, la_index_t, la_object_t) -> la_status_tDeprecated

func sasum_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>) -> Float

func saxpy_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func scasum_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> Float

func scnrm2_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> Float

func scopy_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sdot_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>) -> Float

func sdsdot_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>) -> Float

func sgbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sgemm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sgemv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sger_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func snrm2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>) -> Float

func srot_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>)

func srotg_(UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func srotm_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>)

func srotmg_(UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func ssbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sscal_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sspmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sspr2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func sspr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func sswap_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func ssymm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func ssymv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func ssyr2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func ssyr2k_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func ssyr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func ssyrk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func stbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func stbsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func stpmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func stpsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func strmm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func strmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func strsm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func strsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func xerbla_(UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zaxpy_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zcopy_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zdotc_(OpaquePointer, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zdotu_(OpaquePointer, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zdrot_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>)

func zdscal_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zgbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zgemm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zgemv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zgerc_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zgeru_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zhbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zhemm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zhemv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zher2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zher2k_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zher_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zherk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zhpmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zhpr2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zhpr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zrotg_(OpaquePointer, OpaquePointer, UnsafeMutablePointer&lt;Double>, OpaquePointer)

func zscal_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zswap_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zsymm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zsyr2k_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zsyrk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ztbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ztbsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ztpmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ztpsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ztrmm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ztrmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ztrsm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ztrsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func caxpby_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cbbcsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cbdsqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgbbrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgbequ_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgbequb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgbsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgbsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgbtf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgbtrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgebak_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgebal_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgebd2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgebrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgecon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeequ_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeequb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgees_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_cgees_func_ptr!, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeesx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_cgees_func_ptr!, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgegs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgegv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgehd2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgehrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgejsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgelq2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgelq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgelqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgelqt3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgelqt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgels_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgelsd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgelss_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgelst_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgelsx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgelsy_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgemlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgemlqt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgemqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgemqrt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeql2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeqlf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeqp3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeqpf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeqr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeqr2p_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeqrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeqrfp_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeqrt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeqrt3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgeqrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgerfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgerq2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgerqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgesc2_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>)

func cgesdd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgesv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgesvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgesvdq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgesvdx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgesvj_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgesvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgetc2_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgetf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgetrf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgetrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgetri_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgetrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgetsls_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgetsqrhrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggbak_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggbal_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgges3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_cgges_func_ptr!, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgges_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_cgges_func_ptr!, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggesx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_cgges_func_ptr!, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggev3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggglm_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgghd3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgghrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgglse_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggqrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggrqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggsvd3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggsvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggsvp3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cggsvp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgsvj0_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgsvj1_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgtcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgtrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgtsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgtsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgttrf_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgttrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cgtts2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func chb2st_kernels_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func chbev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chbev_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chbevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chbevd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chbevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chbevx_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chbgst_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chbgv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chbgvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chbgvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chbtrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func checon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func checon_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func checon_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cheequb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cheev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cheev_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cheevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cheevd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cheevr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cheevr_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cheevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cheevx_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chegs2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chegst_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chegv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chegv_2stage_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chegvd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chegvx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cherfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chesv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chesv_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chesv_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chesv_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chesv_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chesvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cheswapr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>)

func chetd2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetf2_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetf2_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrd_hb2st_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrd_he2hb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrf_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrf_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrf_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetri2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetri2x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetri_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetri_3x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetri_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrs2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrs_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrs_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrs_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chetrs_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chfrk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?)

func chgeqz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chla_transtype_(UnsafeMutablePointer&lt;CChar>, __LAPACK_int, UnsafePointer&lt;__LAPACK_int>)

func chpcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func chpev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chpevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chpevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chpgst_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chpgv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chpgvd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chpgvx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chpsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chpsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chptrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chptrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func chptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func chsein_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func chseqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cla_gbamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func cla_gbrcond_c_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_gbrcond_x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_gbrpvgrw_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> Float

func cla_geamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func cla_gercond_c_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_gercond_x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_gerpvgrw_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> Float

func cla_heamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func cla_hercond_c_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_hercond_x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_herpvgrw_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_lin_berr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?)

func cla_porcond_c_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_porcond_x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_porpvgrw_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_syamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func cla_syrcond_c_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_syrcond_x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_syrpvgrw_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?) -> Float

func cla_wwaddw_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?)

func clabrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clacgv_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clacn2_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func clacon_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clacp2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clacpy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clacrm_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func clacrt_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer)

func cladiv_(OpaquePointer, OpaquePointer, OpaquePointer)

func claed0_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func claed7_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func claed8_(UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func claein_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func claesy_(OpaquePointer, OpaquePointer, OpaquePointer, OpaquePointer, OpaquePointer, OpaquePointer, OpaquePointer, OpaquePointer)

func claev2_(OpaquePointer, OpaquePointer, OpaquePointer, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer)

func clag2z_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clags2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;Float>, OpaquePointer, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, OpaquePointer, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;Float>, OpaquePointer)

func clagtm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clahef_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clahef_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func clahef_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clahef_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clahqr_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clahr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clahrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func claic1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Float>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;Float>, OpaquePointer, OpaquePointer)

func clals0_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func clalsa_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func clalsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func clamswlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clamtsqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clangb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func clange_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func clangt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?) -> Float

func clanhb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func clanhe_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func clanhf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>?) -> Float

func clanhp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>?) -> Float

func clanhs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func clanht_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, OpaquePointer?) -> Float

func clansb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func clansp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>?) -> Float

func clansy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func clantb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func clantp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>?) -> Float

func clantr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func clapll_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>)

func clapmr_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func clapmt_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func claqgb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func claqge_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func claqhb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func claqhe_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func claqhp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func claqp2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?)

func claqps_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func claqr0_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func claqr1_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer, OpaquePointer?)

func claqr2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func claqr3_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func claqr4_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func claqr5_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func claqsb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func claqsp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func claqsy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func claqz0_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func claqz1_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func claqz2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func claqz3_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clar1v_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?)

func clar2v_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clarcm_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func clarf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func clarfb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func clarfb_gett_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func clarfg_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer)

func clarfgp_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer)

func clarfp_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer)

func clarft_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clarfx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func clarfy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func clargv_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func clarnv_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func clarrv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func clarscl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clartg_(OpaquePointer, OpaquePointer, UnsafeMutablePointer&lt;Float>, OpaquePointer, OpaquePointer)

func clartv_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clarz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func clarzb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func clarzt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clascl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clascl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func claset_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clasr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func classq_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func claswlq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func claswp_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>)

func clasyf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clasyf_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func clasyf_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clasyf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clatbs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func clatdf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?)

func clatps_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func clatrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func clatrs3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clatrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func clatrz_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?)

func clatsqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clatzm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func claunhr_col_getrfnp2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func claunhr_col_getrfnp_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func clauu2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func clauum_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpbequ_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpbstf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpbsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpbsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpbtf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpbtrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpftrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpftri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpftrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpocon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpoequ_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpoequb_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cporfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cposv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cposvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpotf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpotrf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpotrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpotri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpotrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cppcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cppequ_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cppsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cppsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpptrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpstf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpstrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cptcon_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpteqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cptrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cptsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cptsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, OpaquePointer?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpttrf_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cpttrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cptts2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func crot_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer)

func cspcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cspmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cspr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func csprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cspsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cspsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func csptrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func csptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func csptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csrscl_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cstedc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cstegr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cstein_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cstemr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csteqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csycon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func csycon_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func csycon_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func csyconv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func csyconvf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func csyconvf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func csyequb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func csymv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func csyr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func csyrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func csysv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csysv_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csysv_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csysv_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csysv_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csysvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func csyswapr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>)

func csytf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytf2_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytf2_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytrf_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytrf_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytrf_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytrf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytri2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytri2x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytri_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytri_3x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytri_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytrs2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytrs_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytrs_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytrs_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func csytrs_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctfsm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ctftri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctfttp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctfttr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctgevc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctgex2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctgexc_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctgsen_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctgsja_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctgsna_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctgsy2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctgsyl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctpcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctplqt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctplqt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctpmlqt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctpmqrt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctpqrt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctpqrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctprfb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func ctprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctpttf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctpttr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrevc3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrevc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrexc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrsen_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrsna_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrsyl3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrsyl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrti2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrtri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrttf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctrttp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctzrqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ctzrzf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunbdb1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunbdb2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunbdb3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunbdb4_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunbdb5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunbdb6_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunbdb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cuncsd2by1_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cuncsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cung2l_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cung2r_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cungbr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunghr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cungl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunglq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cungql_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cungqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cungr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cungrq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cungtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cungtsqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cungtsqr_row_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunhr_col_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunm22_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunm2l_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunm2r_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunmbr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunmhr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunml2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunmlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunmql_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunmqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunmr2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunmr3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunmrq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunmrz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cunmtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func cupgtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func cupmtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func daxpby_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dbbcsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dbdsdc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dbdsqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dbdsvdx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dcombssq_(UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>?)

func ddisna_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgbbrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgbequ_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgbequb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgbsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgbsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgbtf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgbtrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgebak_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgebal_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgebd2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgebrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgecon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeequ_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeequb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgees_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_dgees_func_ptr!, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeesx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_dgees_func_ptr!, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgegs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgegv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgehd2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgehrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgejsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgelq2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgelq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgelqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgelqt3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgelqt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgels_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgelsd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgelss_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgelst_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgelsx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgelsy_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgemlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgemlqt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgemqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgemqrt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeql2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeqlf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeqp3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeqpf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeqr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeqr2p_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeqrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeqrfp_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeqrt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeqrt3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgeqrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgerfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgerq2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgerqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgesc2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>)

func dgesdd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgesv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgesvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgesvdq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgesvdx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgesvj_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgesvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgetc2_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgetf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgetrf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgetrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgetri_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgetrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgetsls_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgetsqrhrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggbak_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggbal_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgges3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_dgges_func_ptr!, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgges_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_dgges_func_ptr!, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggesx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_dgges_func_ptr!, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggev3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggglm_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgghd3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgghrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgglse_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggqrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggrqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggsvd3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggsvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggsvp3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dggsvp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgsvj0_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgsvj1_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgtcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgtrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgtsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgtsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgttrf_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgttrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dgtts2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dhgeqz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dhsein_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dhseqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func disnan_(UnsafePointer&lt;Double>) -> __LAPACK_bool

func dla_gbamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dla_gbrcond_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?) -> Double

func dla_gbrpvgrw_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>) -> Double

func dla_geamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dla_gercond_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?) -> Double

func dla_gerpvgrw_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>) -> Double

func dla_lin_berr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?)

func dla_porcond_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?) -> Double

func dla_porpvgrw_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func dla_syamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dla_syrcond_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?) -> Double

func dla_syrpvgrw_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?) -> Double

func dla_wwaddw_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>?)

func dlabad_(UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlabrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlacn2_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func dlacon_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlacpy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dladiv1_(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dladiv2_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>) -> Double

func dladiv_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlae2_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlaebz_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaed0_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaed1_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaed2_(UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaed3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaed4_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaed5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlaed6_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaed7_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaed8_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaed9_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaeda_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaein_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaev2_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlaexc_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlag2_(UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlag2s_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlags2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlagtf_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlagtm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlagts_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlagv2_(UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlahqr_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlahr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlahrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlaic1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlaisnan_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>) -> __LAPACK_bool

func dlaln2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlals0_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlalsa_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlalsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlamc1_(UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_bool>)

func dlamc2_(UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>)

func dlamc3_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>) -> Double

func dlamc4_(UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>)

func dlamc5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>)

func dlamch_(UnsafePointer&lt;CChar>) -> Double

func dlamrg_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func dlamswlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlamtsqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaneg_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func dlangb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func dlange_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func dlangt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?) -> Double

func dlanhs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func dlansb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func dlansf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?) -> Double

func dlansp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?) -> Double

func dlanst_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?) -> Double

func dlansy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func dlantb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func dlantp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?) -> Double

func dlantr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func dlanv2_(UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlaorhr_col_getrfnp2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaorhr_col_getrfnp_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlapll_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>)

func dlapmr_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func dlapmt_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func dlapy2_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>) -> Double

func dlapy3_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>) -> Double

func dlaqgb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func dlaqge_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func dlaqp2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?)

func dlaqps_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlaqr0_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaqr1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?)

func dlaqr2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>)

func dlaqr3_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>)

func dlaqr4_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaqr5_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlaqsb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func dlaqsp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func dlaqsy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func dlaqtr_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaqz0_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaqz1_(UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?)

func dlaqz2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlaqz3_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaqz4_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlar1v_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?)

func dlar2v_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlarf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func dlarfb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>)

func dlarfb_gett_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>)

func dlarfg_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>)

func dlarfgp_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>)

func dlarfp_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>)

func dlarft_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlarfx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func dlarfy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func dlargv_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlarmm_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>) -> Double

func dlarnv_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func dlarra_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlarrb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlarrc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlarrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlarre_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlarrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlarrj_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlarrk_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlarrr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlarrv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlarscl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlartg_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlartgp_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlartgs_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlartv_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlaruv_(UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func dlarz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func dlarzb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>)

func dlarzt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlas2_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlascl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlascl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasd0_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasd1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasd2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasd3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasd4_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasd5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?)

func dlasd6_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasd7_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasd8_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasda_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasdq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasdt_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>)

func dlaset_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlasq1_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasq2_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasq3_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlasq4_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>)

func dlasq5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;Double>)

func dlasq6_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlasr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlasrt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlassq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlasv2_(UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func dlaswlq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlaswp_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>)

func dlasy2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasyf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasyf_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func dlasyf_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlasyf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlat2s_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlatbs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlatdf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?)

func dlatps_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlatrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dlatrs3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlatrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlatrz_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?)

func dlatsqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlatzm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func dlauu2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dlauum_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dopgtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dopmtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorbdb1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorbdb2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorbdb3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorbdb4_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorbdb5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorbdb6_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorbdb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorcsd2by1_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorcsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorg2l_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorg2r_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorgbr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorghr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorgl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorglq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorgql_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorgqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorgr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorgrq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorgtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorgtsqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorgtsqr_row_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorhr_col_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorm22_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorm2l_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorm2r_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dormbr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dormhr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dorml2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dormlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dormql_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dormqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dormr2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dormr3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dormrq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dormrz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dormtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpbequ_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpbstf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpbsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpbsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpbtf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpbtrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpftrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpftri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpftrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpocon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpoequ_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpoequb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dporfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dposv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dposvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpotf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpotrf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpotrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpotri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpotrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dppcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dppequ_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dppsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dppsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpptrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpstf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpstrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dptcon_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpteqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dptrfs_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dptsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dptsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpttrf_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dpttrs_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dptts2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func drscl_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dsb2st_kernels_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func dsbev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsbev_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsbevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsbevd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsbevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsbevx_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsbgst_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsbgv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsbgvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsbgvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsbtrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsfrk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?)

func dsgesv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dspcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dspev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dspevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dspevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dspgst_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dspgv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dspgvd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dspgvx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsposv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dspsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dspsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsptrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsptrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dstebz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dstedc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dstegr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dstein_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dstemr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsteqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsterf_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dstev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dstevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dstevr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dstevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsycon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsycon_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsycon_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyconv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyconvf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyconvf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyequb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyev_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyevd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyevr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyevr_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyevx_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsygs2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsygst_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsygv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsygv_2stage_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsygvd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsygvx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsysv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsysv_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsysv_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsysv_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsysv_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsysvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsyswapr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>)

func dsytd2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytf2_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytf2_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrd_sb2st_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrd_sy2sb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrf_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrf_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrf_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytri2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytri2x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytri_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytri_3x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytri_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrs2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrs_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrs_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrs_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dsytrs_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtfsm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func dtftri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtfttp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtfttr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtgevc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtgex2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtgexc_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtgsen_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtgsja_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtgsna_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtgsy2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtgsyl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtpcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtplqt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtplqt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtpmlqt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtpmqrt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtpqrt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtpqrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtprfb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>)

func dtprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtpttf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtpttr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrevc3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrevc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrexc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrsen_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrsna_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrsyl3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrsyl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrti2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrtri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrttf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtrttp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtzrqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func dtzrzf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func dzsum1_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> Double

func icmax1_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func ieeeck_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>) -> __LAPACK_int

func ilaclc_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func ilaclr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func iladiag_(UnsafePointer&lt;CChar>) -> __LAPACK_int

func iladlc_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func iladlr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func ilaenv2stage_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func ilaenv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func ilaprec_(UnsafePointer&lt;CChar>) -> __LAPACK_int

func ilaslc_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func ilaslr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func ilatrans_(UnsafePointer&lt;CChar>) -> __LAPACK_int

func ilauplo_(UnsafePointer&lt;CChar>) -> __LAPACK_int

func ilaver_(UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ilazlc_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func ilazlr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func iparam2stage_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func iparmq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func izmax1_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func lsamen_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>) -> __LAPACK_bool

func saxpby_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sbbcsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sbdsdc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sbdsqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sbdsvdx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func scombssq_(UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>?)

func scsum1_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> Float

func sdisna_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgbbrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgbequ_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgbequb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgbsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgbsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgbtf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgbtrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgebak_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgebal_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgebd2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgebrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgecon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeequ_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeequb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgees_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_sgees_func_ptr!, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeesx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_sgees_func_ptr!, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgegs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgegv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgehd2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgehrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgejsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgelq2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgelq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgelqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgelqt3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgelqt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgels_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgelsd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgelss_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgelst_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgelsx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgelsy_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgemlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgemlqt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgemqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgemqrt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeql2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeqlf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeqp3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeqpf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeqr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeqr2p_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeqrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeqrfp_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeqrt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeqrt3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgeqrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgerfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgerq2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgerqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgesc2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>)

func sgesdd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgesv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgesvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgesvdq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgesvdx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgesvj_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgesvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgetc2_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgetf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgetrf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgetrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgetri_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgetrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgetsls_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgetsqrhrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggbak_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggbal_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgges3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_sgges_func_ptr!, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgges_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_sgges_func_ptr!, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggesx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_sgges_func_ptr!, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggev3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggglm_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgghd3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgghrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgglse_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggqrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggrqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggsvd3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggsvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggsvp3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sggsvp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgsvj0_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgsvj1_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgtcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgtrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgtsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgtsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgttrf_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgttrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sgtts2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func shgeqz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func shsein_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func shseqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sisnan_(UnsafePointer&lt;Float>) -> __LAPACK_bool

func sla_gbamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sla_gbrcond_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?) -> Float

func sla_gbrpvgrw_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>) -> Float

func sla_geamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sla_gercond_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?) -> Float

func sla_gerpvgrw_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>) -> Float

func sla_lin_berr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?)

func sla_porcond_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?) -> Float

func sla_porpvgrw_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func sla_syamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sla_syrcond_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?) -> Float

func sla_syrpvgrw_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?) -> Float

func sla_wwaddw_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>?)

func slabad_(UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slabrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slacn2_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func slacon_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slacpy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func sladiv1_(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func sladiv2_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>) -> Float

func sladiv_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slae2_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slaebz_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaed0_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaed1_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaed2_(UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaed3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaed4_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaed5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slaed6_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaed7_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaed8_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaed9_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaeda_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaein_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaev2_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slaexc_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slag2_(UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slag2d_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slags2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slagtf_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slagtm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slagts_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slagv2_(UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slahqr_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slahr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slahrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slaic1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slaisnan_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>) -> __LAPACK_bool

func slaln2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slals0_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slalsa_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slalsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slamc1_(UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_bool>)

func slamc2_(UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>)

func slamc3_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>) -> Float

func slamc4_(UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>)

func slamc5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>)

func slamch_(UnsafePointer&lt;CChar>) -> Float

func slamrg_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func slamswlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slamtsqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaneg_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>) -> __LAPACK_int

func slangb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func slange_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func slangt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?) -> Float

func slanhs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func slansb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func slansf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?) -> Float

func slansp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?) -> Float

func slanst_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?) -> Float

func slansy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func slantb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func slantp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?) -> Float

func slantr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?) -> Float

func slanv2_(UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slaorhr_col_getrfnp2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaorhr_col_getrfnp_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slapll_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>)

func slapmr_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func slapmt_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func slapy2_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>) -> Float

func slapy3_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>) -> Float

func slaqgb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func slaqge_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func slaqp2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?)

func slaqps_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slaqr0_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaqr1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?)

func slaqr2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>)

func slaqr3_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>)

func slaqr4_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaqr5_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slaqsb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func slaqsp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func slaqsy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;CChar>)

func slaqtr_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaqz0_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaqz1_(UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?)

func slaqz2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slaqz3_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaqz4_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slar1v_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?)

func slar2v_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slarf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func slarfb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>)

func slarfb_gett_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>)

func slarfg_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>)

func slarfgp_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>)

func slarfp_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>)

func slarft_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slarfx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func slarfy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func slargv_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slarmm_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>) -> Float

func slarnv_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func slarra_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slarrb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slarrc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slarrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slarre_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slarrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slarrj_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slarrk_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slarrr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slarrv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slarscl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slartg_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slartgp_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slartgs_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slartv_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slaruv_(UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func slarz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func slarzb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>)

func slarzt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slas2_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slascl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slascl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasd0_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasd1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasd2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasd3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasd4_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasd5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?)

func slasd6_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasd7_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasd8_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasda_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasdq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasdt_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>)

func slaset_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slasq1_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasq2_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasq3_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slasq4_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>)

func slasq5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;Float>)

func slasq6_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slasr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slasrt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slassq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slasv2_(UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

func slaswlq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slaswp_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>)

func slasy2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasyf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasyf_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func slasyf_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slasyf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slatbs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slatdf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?)

func slatps_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slatrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func slatrs3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slatrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func slatrz_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?)

func slatsqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slatzm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func slauu2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func slauum_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sopgtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sopmtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorbdb1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorbdb2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorbdb3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorbdb4_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorbdb5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorbdb6_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorbdb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorcsd2by1_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorcsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorg2l_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorg2r_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorgbr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorghr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorgl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorglq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorgql_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorgqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorgr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorgrq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorgtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorgtsqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorgtsqr_row_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorhr_col_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorm22_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorm2l_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorm2r_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sormbr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sormhr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sorml2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sormlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sormql_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sormqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sormr2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sormr3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sormrq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sormrz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sormtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func spbequ_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func spbstf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spbsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spbsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func spbtf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spbtrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spftrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func spftri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func spftrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spocon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func spoequ_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spoequb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sporfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sposv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sposvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func spotf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spotrf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spotrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spotri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spotrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sppcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sppequ_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sppsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sppsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func spptrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func spptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func spptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spstf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spstrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sptcon_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spteqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sptrfs_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sptsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sptsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func spttrf_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func spttrs_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sptts2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func srscl_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func ssb2st_kernels_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?)

func ssbev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssbev_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssbevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssbevd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssbevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssbevx_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssbgst_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssbgv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssbgvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssbgvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssbtrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssfrk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?)

func sspcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sspev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sspevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sspevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sspgst_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sspgv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sspgvd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sspgvx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sspsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sspsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssptrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssptrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sstebz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sstedc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sstegr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sstein_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sstemr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssteqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssterf_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func sstev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sstevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sstevr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func sstevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssycon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssycon_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssycon_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyconv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyconvf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyconvf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyequb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyev_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyevd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyevr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyevr_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyevx_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssygs2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssygst_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssygv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssygv_2stage_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssygvd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssygvx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssysv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssysv_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssysv_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssysv_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssysv_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssysvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssyswapr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>)

func ssytd2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytf2_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytf2_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrd_sb2st_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrd_sy2sb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrf_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrf_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrf_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytri2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytri2x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytri_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytri_3x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytri_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrs2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrs_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrs_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrs_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ssytrs_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stfsm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>)

func stftri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stfttp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stfttr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stgevc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stgex2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stgexc_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stgsen_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stgsja_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stgsna_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stgsy2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stgsyl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stpcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stplqt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stplqt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stpmlqt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stpmqrt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stpqrt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stpqrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stprfb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>)

func stprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func stpttf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stpttr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func strcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func strevc3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func strevc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func strexc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func strrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func strsen_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func strsna_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func strsyl3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func strsyl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;__LAPACK_int>)

func strti2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func strtri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func strtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func strttf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func strttp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stzrqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func stzrzf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func vcospif(vFloat) -> vFloat

func vsinpif(vFloat) -> vFloat

func vtanpif(vFloat) -> vFloat

func zaxpby_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zbbcsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zbdsqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zcgesv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zcposv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zdrscl_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zgbbrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgbequ_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgbequb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgbsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgbsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgbtf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgbtrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgebak_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgebal_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgebd2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgebrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgecon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeequ_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeequb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgees_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_zgees_func_ptr!, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeesx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_zgees_func_ptr!, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgegs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgegv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgehd2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgehrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgejsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgelq2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgelq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgelqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgelqt3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgelqt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgels_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgelsd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgelss_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgelst_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgelsx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgelsy_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgemlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgemlqt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgemqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgemqrt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeql2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeqlf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeqp3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeqpf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeqr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeqr2p_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeqrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeqrfp_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeqrt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeqrt3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgeqrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgerfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgerq2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgerqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgesc2_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>)

func zgesdd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgesv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgesvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgesvdq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgesvdx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgesvj_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgesvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgetc2_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgetf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgetrf2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgetrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgetri_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgetrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgetsls_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgetsqrhrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggbak_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggbal_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgges3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_zgges_func_ptr!, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgges_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_zgges_func_ptr!, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggesx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, __LAPACK_zgges_func_ptr!, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggev3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_bool>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggglm_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgghd3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgghrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgglse_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggqrf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggrqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggsvd3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggsvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggsvp3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zggsvp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgsvj0_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgsvj1_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgtcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgtrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgtsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgtsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgttrf_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgttrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zgtts2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zhb2st_kernels_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zhbev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhbev_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhbevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhbevd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhbevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhbevx_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhbgst_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhbgv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhbgvd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhbgvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhbtrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhecon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhecon_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhecon_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zheequb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zheev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zheev_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zheevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zheevd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zheevr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zheevr_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zheevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zheevx_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhegs2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhegst_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhegv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhegv_2stage_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhegvd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhegvx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zherfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhesv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhesv_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhesv_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhesv_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhesv_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhesvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zheswapr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>)

func zhetd2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetf2_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetf2_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrd_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrd_hb2st_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrd_he2hb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrf_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrf_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrf_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetri2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetri2x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetri_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetri_3x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetri_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrs2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrs_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrs_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrs_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhetrs_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhfrk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?)

func zhgeqz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhpcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhpev_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhpevd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhpevx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhpgst_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhpgv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhpgvd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhpgvx_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhpsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhpsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhptrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhptrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhsein_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zhseqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zla_gbamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func zla_gbrcond_c_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_gbrcond_x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_gbrpvgrw_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> Double

func zla_geamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func zla_gercond_c_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_gercond_x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_gerpvgrw_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>) -> Double

func zla_heamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func zla_hercond_c_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_hercond_x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_herpvgrw_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_lin_berr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?)

func zla_porcond_c_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_porcond_x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_porpvgrw_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_syamv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func zla_syrcond_c_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_syrcond_x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_syrpvgrw_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?) -> Double

func zla_wwaddw_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?)

func zlabrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlacgv_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlacn2_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func zlacon_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlacp2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlacpy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlacrm_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func zlacrt_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer)

func zladiv_(OpaquePointer, OpaquePointer, OpaquePointer)

func zlaed0_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlaed7_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlaed8_(UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlaein_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlaesy_(OpaquePointer, OpaquePointer, OpaquePointer, OpaquePointer, OpaquePointer, OpaquePointer, OpaquePointer, OpaquePointer)

func zlaev2_(OpaquePointer, OpaquePointer, OpaquePointer, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer)

func zlag2c_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlags2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;Double>, OpaquePointer, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, OpaquePointer, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;Double>, OpaquePointer)

func zlagtm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlahef_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlahef_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zlahef_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlahef_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlahqr_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlahr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlahrd_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlaic1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Double>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;Double>, OpaquePointer, OpaquePointer)

func zlals0_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlalsa_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlalsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlamswlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlamtsqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlangb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func zlange_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func zlangt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?) -> Double

func zlanhb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func zlanhe_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func zlanhf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>?) -> Double

func zlanhp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>?) -> Double

func zlanhs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func zlanht_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, OpaquePointer?) -> Double

func zlansb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func zlansp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>?) -> Double

func zlansy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func zlantb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func zlantp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>?) -> Double

func zlantr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?) -> Double

func zlapll_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>)

func zlapmr_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func zlapmt_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?)

func zlaqgb_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func zlaqge_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func zlaqhb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func zlaqhe_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func zlaqhp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func zlaqp2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?)

func zlaqps_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlaqr0_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlaqr1_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer, OpaquePointer?)

func zlaqr2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func zlaqr3_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func zlaqr4_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlaqr5_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlaqsb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func zlaqsp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func zlaqsy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;CChar>)

func zlaqz0_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlaqz1_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlaqz2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlaqz3_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlar1v_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, OpaquePointer?, UnsafePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?)

func zlar2v_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlarcm_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?)

func zlarf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zlarfb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func zlarfb_gett_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func zlarfg_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer)

func zlarfgp_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer)

func zlarfp_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer)

func zlarft_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlarfx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zlarfy_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zlargv_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>)

func zlarnv_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zlarrv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlarscl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlartg_(OpaquePointer, OpaquePointer, UnsafeMutablePointer&lt;Double>, OpaquePointer, OpaquePointer)

func zlartv_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlarz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zlarzb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func zlarzt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlascl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlascl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlaset_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlasr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlassq_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

func zlaswlq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlaswp_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>)

func zlasyf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlasyf_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zlasyf_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlasyf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlat2c_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlatbs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlatdf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?)

func zlatps_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlatrd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zlatrs3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlatrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlatrz_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?)

func zlatsqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlatzm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zlaunhr_col_getrfnp2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlaunhr_col_getrfnp_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlauu2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zlauum_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpbequ_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpbstf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpbsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpbsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpbtf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpbtrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpftrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpftri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpftrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpocon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpoequ_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpoequb_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zporfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zposv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zposvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpotf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpotrf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpotrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpotri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpotrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zppcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zppequ_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zppsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zppsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpptrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpstf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpstrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zptcon_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpteqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zptrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zptsv_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zptsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, OpaquePointer?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpttrf_(UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zpttrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zptts2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zrot_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, OpaquePointer)

func zspcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zspmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zspr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?)

func zsprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zspsv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zspsvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsptrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zstedc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zstegr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zstein_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zstemr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_bool>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsteqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsycon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsycon_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsycon_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsyconv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsyconvf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsyconvf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsyequb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsymv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zsyr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func zsyrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsysv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsysv_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsysv_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsysv_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsysv_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsysvx_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsyswapr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>)

func zsytf2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytf2_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytf2_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytrf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytrf_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytrf_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytrf_rk_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytrf_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytri2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytri2x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytri_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytri_3x_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytri_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytrs2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytrs_3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytrs_aa_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytrs_aa_2stage_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zsytrs_rook_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztbcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztbrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztbtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztfsm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ztftri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztfttp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztfttr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztgevc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztgex2_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztgexc_(UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztgsen_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztgsja_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztgsna_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztgsy2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztgsyl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztpcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztplqt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztplqt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztpmlqt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztpmqrt_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztpqrt2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztpqrt_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztprfb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>)

func ztprfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztptri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztptrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztpttf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztpttr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrcon_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrevc3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrevc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrexc_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrrfs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrsen_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrsna_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_bool>?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrsyl3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrsyl_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrti2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrtri_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrtrs_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrttf_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztrttp_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztzrqf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func ztzrzf_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunbdb1_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunbdb2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunbdb3_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunbdb4_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunbdb5_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunbdb6_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunbdb_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zuncsd2by1_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zuncsd_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;Double>?, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zung2l_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zung2r_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zungbr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunghr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zungl2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunglq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zungql_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zungqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zungr2_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zungrq_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zungtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zungtsqr_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zungtsqr_row_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunhr_col_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunm22_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunm2l_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunm2r_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunmbr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunmhr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunml2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunmlq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunmql_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunmqr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunmr2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunmr3_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunmrq_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunmrz_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zunmtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafePointer&lt;__LAPACK_int>, UnsafeMutablePointer&lt;__LAPACK_int>)

func zupgtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

func zupmtr_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, OpaquePointer?, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, UnsafeMutablePointer&lt;__LAPACK_int>)

