

- Kernel
- Kernel Functions
-  vn_bwrite 

Function

# vn_bwrite

System-provided implementation of "bwrite" vnop.

macOS 10.4+

``` source
int vn_bwrite(struct vnop_bwrite_args *ap);
```

## Parameters 

`ap`  

Standard parameters to a bwrite vnop.

## Return Value

Results of buf_bwrite directly.

## Discussion

This routine is available for filesystems which do not want to implement their own "bwrite" vnop. It just calls buf_bwrite() without modifying its arguments.

