

- Accelerate
-  SparseGetInertia(\_:\_:\_:\_:) 

Function

# SparseGetInertia(\_:\_:\_:\_:)

Returns the inertia of a double-precision *LDLᵀ* factorization.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func SparseGetInertia(
    _ Factored: SparseOpaqueFactorization_Double,
    _ num_positive: UnsafeMutablePointer,
    _ num_zero: UnsafeMutablePointer,
    _ num_negative: UnsafeMutablePointer
) -> Int32
```

## Parameters 

`Factored`  

The SparseFactorizationLDLTTPP factorization.

`num_positive`  

On return, the number of positive pivots the sparse factorization functions take during the factorization of `Factored`.

`num_zero`  

On return, the number of zero pivots the sparse factorization functions take during the factorization of `Factored`.

`num_negative`  

On return, the number of negative pivots the sparse factorization functions take during the factorization of `Factored`.

## Return Value

`0` on success; otherwise, a nonzero value on error.

## Discussion

This function returns the number of negative, zero, and positive pivots that the sparse factorization functions, SparseFactor(_:_:) and SparseFactor(_:_:_:_:), take during an *LDLᵀ* factorization.

In some cases — for example, when the original matrix’s eigenvalues are close to zero — the computed numerical inertia may not be an accurate reflection of the true inertia. In such cases, the computed numerical inertia is dependent on the zeroTolerance and pivotTolerance values of the SparseNumericFactorOptions structure.

Important

This function supports only SparseFactorizationLDLTTPP factorizations.

## See Also

### Factorization Intertia Functions

func SparseGetInertia(SparseOpaqueFactorization_Float, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;Int32>) -> Int32

Returns the inertia of a single-precision *LDLᵀ* factorization.

