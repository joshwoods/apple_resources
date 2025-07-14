

- Kernel
- Deprecated Symbols
-  mbuf_setdata Deprecated

Function

# mbuf_setdata

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_setdata(mbuf_t mbuf, void *data, size_t len);
```

## Parameters 

`mbuf`  

The mbuf.

`data`  

The new pointer value for data.

`len`  

The new length of data in the mbuf.

## Return Value

0 on success, errno error on failure.

## Discussion

Sets the data and length values for an mbuf. The data value must be in a valid range. In the case of an mbuf with a cluster, the data value must point to a location in the cluster and the data value plus the length, must be less than the end of the cluster. For data embedded directly in an mbuf (no cluster), the data value must fall somewhere between the start and end of the data area in the mbuf and the data + length must also be in the same range.

