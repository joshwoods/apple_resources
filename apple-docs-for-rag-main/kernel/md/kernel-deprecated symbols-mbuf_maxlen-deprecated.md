

- Kernel
- Deprecated Symbols
-  mbuf_maxlen Deprecated

Function

# mbuf_maxlen

macOS 10.4–10.15.4Deprecated

``` source
size_t mbuf_maxlen(const mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf.

## Return Value

The maximum lenght of data for this mbuf.

## Discussion

Retrieves the maximum length of data that may be stored in this mbuf. This value assumes that the data pointer was set to the start of the possible range for that pointer (mbuf_data_start).

