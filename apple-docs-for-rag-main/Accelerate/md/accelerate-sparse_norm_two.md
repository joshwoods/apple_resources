

- Accelerate
-  SPARSE_NORM_TWO 

Global Variable

# SPARSE_NORM_TWO

Norm Two

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var SPARSE_NORM_TWO: sparse_norm { get }
```

## Discussion

| Matrix element wise | *sqrt( sumᵢ,ⱼ (A\[i,j\])² )*\_\_ |
|----|----|
| Matrix operator | Largest singular value of matrix, note that the operator SPARSE_NORM_TWO is significantly more expensive than other norm operations.\_\_ |
| Vector element wise | *sqrt( sumᵢ (x\[i\])² )*\_\_ |

## See Also

### Constants

var SPARSE_NORM_ONE: sparse_norm

Norm One

var SPARSE_NORM_INF: sparse_norm

Norm Inf

var SPARSE_NORM_R1: sparse_norm

Norm R1

