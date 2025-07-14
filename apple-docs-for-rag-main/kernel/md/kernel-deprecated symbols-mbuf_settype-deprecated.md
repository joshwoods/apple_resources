

- Kernel
- Deprecated Symbols
-  mbuf_settype Deprecated

Function

# mbuf_settype

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_settype(mbuf_t mbuf, mbuf_type_t new_type);
```

## Parameters 

`mbuf`  

The mbuf.

`new_type`  

The new type.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Sets the type of mbuf.

