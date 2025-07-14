

- Accelerate
-  SparseOrderAMD 

Global Variable

# SparseOrderAMD

Approximate minimum degree (AMD) ordering.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var SparseOrderAMD: SparseOrder_t { get }
```

## Discussion

There’s a large overhead cost if you use this for QR-based factorization due to explicit formation of *AᵀA*.

## See Also

### Constants

var SparseOrderDefault: SparseOrder_t

The default ordering.

var SparseOrderUser: SparseOrder_t

The user-supplied ordering, or identity if the order parameter is null.

var SparseOrderMetis: SparseOrder_t

METIS nested dissection ordering.

var SparseOrderCOLAMD: SparseOrder_t

The column AMD ordering for *AᵀA*.

