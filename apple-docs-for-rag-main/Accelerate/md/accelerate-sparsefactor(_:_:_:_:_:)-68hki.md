

- Accelerate
-  SparseFactor(\_:\_:\_:\_:\_:) 

Function

# SparseFactor(\_:\_:\_:\_:\_:)

Returns the factorization of a sparse matrix of double-precision values that corresponds to the supplied symbolic factorization using user-defined workspace and factor storage.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseFactor(
    _ symbolicFactor: SparseOpaqueSymbolicFactorization,
    _ Matrix: SparseMatrix_Double,
    _ nfoptions: SparseNumericFactorOptions,
    _ factorStorage: UnsafeMutableRawPointer?,
    _ workspace: UnsafeMutableRawPointer?
) -> SparseOpaqueFactorization_Double
```

## Parameters 

`symbolicFactor`  

A symbolic factorization that returns by calling SparseFactor(_:_:_:_:_:).

`Matrix`  

The matrix to factorize.

`nfoptions`  

The numeric factor options, such as pivoting parameters.

`factorStorage`  

A pointer to space for storing the factorization of size at least factorSize_Double bytes. Don’t alter this storage during the lifetime of the return value.

`workspace`  

A pointer to a workspace of size at least workspaceSize_Double bytes. You can reuse or deallocate the workspace storage after the function returns.

## Return Value

A SparseOpaqueFactorization_Double structure that represents the matrix factorization.

## Discussion

Use this function to solve a system of linear equations using a symbolic factorization that SparseFactor(_:_:) creates.

The following code creates the workspace and factor storage that this function requires, and solves this system with a QR factorization of the coefficient matrix:

```
/// Define the sparsity pattern of the coefficient matrix.
let rowIndices: [Int32] =    [ 0, 1, 1, 2]
let columnIndices: [Int32] = [ 2, 0, 2, 1]

/// Create the double-precision coefficient matrix _A_.
let aValues: [Double] = [10, 20, 5, 50]
let A = SparseConvertFromCoordinate(3, 3,
                                    4, 1,
                                    SparseAttributes_t(),
                                    rowIndices, columnIndices,
                                    aValues)

/// Compute the symbolic factorization from the structure of the coefficient matrix.
let structure = A.structure
let symbolicFactorization = SparseFactor(SparseFactorizationQR,
                                         structure)

/// Create the workspace.
let workspace = UnsafeMutableRawPointer.allocate(
    byteCount: symbolicFactorization.workspaceSize_Double,
    alignment: MemoryLayout.alignment)
defer {
    workspace.deallocate()
}

/// Create the factor storage.
let factorStorage = UnsafeMutableRawPointer.allocate(
    byteCount: symbolicFactorization.factorSize_Double,
    alignment: MemoryLayout.alignment)
defer {
    factorStorage.deallocate()
}

/// Factorize _A_ using the symbolic factorization.
let factorization = SparseFactor(symbolicFactorization, A,
                                 SparseNumericFactorOptions(),
                                 factorStorage, workspace)

/// Solve _Ax = b_ in place.
var b0Values: [Double] = [30, 35, 100]
b0Values.withUnsafeMutableBufferPointer { bPtr in
    let xb = DenseVector_Double(count: 3,
                                data: bPtr.baseAddress!)

    SparseSolve(factorization, xb)
}

SparseCleanup(A)
SparseCleanup(factorization)
```

On return, `bValues` contains the values `[1.0, 2.0, 3.0].`

Note that internal memory allocations may occur in the case of pivoted factorizations that result in delayed pivots. If you require closer control over memory allocations, supply a malloc function that implements the required behavior, or use an alternative that nonpivoted factorization returns. Note that if malloc returns `NULL`, the factorization aborts immediately.

## See Also

### Matrix Factorizations Using Precalculated Symbolic Factorization with User-Defined Workspace

func SparseFactor(SparseOpaqueSymbolicFactorization, SparseMatrix_Float, SparseNumericFactorOptions, UnsafeMutableRawPointer?, UnsafeMutableRawPointer?) -> SparseOpaqueFactorization_Float

Returns the factorization of a sparse matrix of single-precision values that corresponds to the supplied symbolic factorization using user-defined workspace and factor storage.

