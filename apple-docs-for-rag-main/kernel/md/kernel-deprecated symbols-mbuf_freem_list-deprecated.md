

- Kernel
- Deprecated Symbols
-  mbuf_freem_list Deprecated

Function

# mbuf_freem_list

macOS 10.4–10.15.4Deprecated

``` source
int mbuf_freem_list(mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The first mbuf in the linked list to free.

## Return Value

The number of mbufs freed.

## Discussion

Frees linked list of mbuf chains. Walks through mnextpackt and does the equivalent of mbuf_freem to each.

