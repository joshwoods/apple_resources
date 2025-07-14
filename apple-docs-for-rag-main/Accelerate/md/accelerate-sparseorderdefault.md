

- Accelerate
-  SparseOrderDefault 

Global Variable

# SparseOrderDefault

The default ordering.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var SparseOrderDefault: SparseOrder_t { get }
```

## Discussion

The default ordering is SparseOrderAMD for symmetric and SparseOrderCOLAMD for unsymmetric factorizations.

## See Also

### Constants

var SparseOrderUser: SparseOrder_t

The user-supplied ordering, or identity if the order parameter is null.

var SparseOrderAMD: SparseOrder_t

Approximate minimum degree (AMD) ordering.

var SparseOrderMetis: SparseOrder_t

METIS nested dissection ordering.

var SparseOrderCOLAMD: SparseOrder_t

The column AMD ordering for *AᵀA*.

