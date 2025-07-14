

- Accelerate
-  SparseOrderCOLAMD 

Global Variable

# SparseOrderCOLAMD

The column AMD ordering for *AᵀA*.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var SparseOrderCOLAMD: SparseOrder_t { get }
```

## Discussion

This ordering isn’t valid for symmetric factorizations (use SparseOrderAMD instead).

## See Also

### Constants

var SparseOrderDefault: SparseOrder_t

The default ordering.

var SparseOrderUser: SparseOrder_t

The user-supplied ordering, or identity if the order parameter is null.

var SparseOrderAMD: SparseOrder_t

Approximate minimum degree (AMD) ordering.

var SparseOrderMetis: SparseOrder_t

METIS nested dissection ordering.

