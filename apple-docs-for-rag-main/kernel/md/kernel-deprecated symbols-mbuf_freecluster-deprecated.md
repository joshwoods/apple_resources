

- Kernel
- Deprecated Symbols
-  mbuf_freecluster Deprecated

Function

# mbuf_freecluster

macOS 10.4–10.15.4Deprecated

``` source
void mbuf_freecluster(caddr_t addr, size_t size);
```

## Parameters 

`addr`  

The address of the cluster.

`size`  

The actual size of the cluster.

## Discussion

Free a cluster that was previously allocated by a call to mbuf_alloccluster(). The caller must pass the actual size of the cluster as returned by mbuf_alloccluster(), which at this point must be either 2048, 4096 or 16384 bytes.

