

- Accelerate
-  la_solve(\_:\_:) Deprecated

Function

# la_solve(\_:\_:)

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.10–11.0DeprecatedtvOS 8.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–7.0Deprecated

``` source
func la_solve(
    _ matrix_system: la_object_t,
    _ obj_rhs: la_object_t
) -> la_object_t
```

Deprecated

This API is deprecated, please use BLAS and LAPACK

## Parameters 

`matrix_system`  

A matrix describing the left-hand side of the system.

`obj_rhs`  

A vector or matrix describing one or more right-hand sides for which the equations are to be solved.

## Return Value

A matrix of the solution(s) of the system of equations.

## Discussion

Solves a system of linear equations

If matrix_system represents a matrix A, and obj_rhs represents a vector B, la_solve returns a vector X representing a solution to the equation AX = B, if such a solution exists. If obj_rhs represents a matrix, then la_solve returns a matrix representing the solution of the same equation.

There are several different cases, and different algorithms are chosen depending on the specifics:

If the matrix has a special structure that allows us to solve the system without factoring (e.g. if the matrix is diagonal or triangular), we may use that structure to compute the solution.

If the matrix is symmetric and all diagonal entries are positive, or if we know, either via a hint parameter or by how earlier computations were structured, that the matrix is positive definite, we attempt a Cholesky factorization. If this succeeds, it is used to compute the solution via forward- and back-substitution.

If the matrix is square, we try to perform Gaussian elimination to construct a triangular factorization with pivoting. If this factorization succeeds, we use it to solve the system. If it fails, the returned object has the error status LA_SINGULAR_ERROR.

If the matrix is not square, we return a least-squares solution computed by performing a QR factorization of the matrix.

If the number of rows of the matrix does not match the number of rows of the right hand side object, the returned object has status LA_DIMENSION_MISMATCH_ERROR.

If the object describing the matrix is not a matrix, or if the right hand side is not a matrix or vector, the returned object has status LA_INVALID_PARAMETER_ERROR.

If you want to solve the system XA = B, which is less common (but still occurs fairly frequently), you may accomplish this by transposing A and B, solving, and then transposing the result of the solve.

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

