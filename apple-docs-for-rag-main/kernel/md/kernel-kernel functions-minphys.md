

- Kernel
- Kernel Functions
-  minphys 

Function

# minphys

Adjust a buffer's count to be no more than maximum physical I/O transfer size for the host architecture.

macOS 10.4+

``` source
u_int minphys(buf_t bp);
```

## Parameters 

`bp`  

The buffer whose byte count to modify.

## Return Value

New byte count.

## Discussion

physio() takes as a parameter a function to bound transfer sizes for each VNOP_STRATEGY() call. minphys() is a default implementation. It calls buf_setcount() to make the buffer's count the min() of its current count and the max I/O size for the host architecture.

