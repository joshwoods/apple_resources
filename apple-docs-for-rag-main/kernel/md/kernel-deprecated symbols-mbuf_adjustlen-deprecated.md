

- Kernel
- Deprecated Symbols
-  mbuf_adjustlen Deprecated

Function

# mbuf_adjustlen

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_adjustlen(mbuf_t mbuf, int amount);
```

## Parameters 

`mbuf`  

The mbuf to adjust.

`amount`  

The number of bytes increment the length by.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Adds amount to the mbuf len. Verifies that the new length is valid (greater than or equal to zero and less than maximum amount of data that may be stored in the mbuf). This function will not adjust the packet header length field or affect any other mbufs in a chain.

