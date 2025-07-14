

- Accelerate
- SparseSymbolicFactorOptions
-  order 

Instance Property

# order

The user-supplied array for ordering.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var order: UnsafeMutablePointer?
```

## Discussion

This property may be either `null` or a pointer to a permutation that reduces fill in the matrix that you’re factoring. The factor function encodes each element, `i`, as the `order[i]`-th position.

For example, to order columns as `0, 4, 2, 1, 3`, specify this property as `[0, 3, 2, 4, 1]`. That is, the ordering that you specify is the inverse of the column ordering. The following code shows that `order[invp[i]]` equals `i` for all values of `i`:

```
let order = [0, 3, 2, 4, 1]
let invp =  [0, 4, 2, 1, 3]

// Prints "[0, 1, 2, 3, 4]".
print((0 ..

If orderMethod is SparseOrderUser, and this pointer is `null`, the factor function uses the original matrix ordering.

If orderMethod is SparseOrderUser, and this pointer is nonnull, the factor function uses the user-provided permutation to order the matrix before factorization. The system may heuristically reinterpret the order to increase performance. Such reorderings don’t significantly increase fill in the factors *L*.

If orderMethod isn’t SparseOrderUser, the factor function computes its own fill-reducing ordering.

If this pointer is nonnull, the factor function returns the computed permutation in the array. Pivoted factorizations may alter the actual permutation during the numerical factorization step.

## See Also

### Inspecting Symbolic Factor Options

var control: SparseControl_t

The flags that control the computation.

struct SparseControl_t

Options that control the computation.

var orderMethod: SparseOrder_t

The ordering algorithm.

struct SparseOrder_t

Options that define which ordering algorithm to use.

var ignoreRowsAndColumns: UnsafeMutablePointer&lt;Int32>?

An array that contains row and column indices to ignore.

var malloc: (Int) -> UnsafeMutableRawPointer?

The function for allocating any necessary storage.

var free: (UnsafeMutableRawPointer?) -> Void

The function for freeing allocated storage.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

The function for reporting parameter errors.

