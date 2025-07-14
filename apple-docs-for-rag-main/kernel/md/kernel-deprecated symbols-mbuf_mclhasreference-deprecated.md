

- Kernel
- Deprecated Symbols
-  mbuf_mclhasreference Deprecated

Function

# mbuf_mclhasreference

macOS 10.4–10.15.4Deprecated

``` source
int mbuf_mclhasreference(mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf with the cluster to test.

## Return Value

0 if there is no reference by another mbuf, 1 otherwise.

## Discussion

Check if a cluster of an mbuf is referenced by another mbuf. References may be taken, for example, as a result of a call to mbuf_split or mbuf_copym

