

- Kernel
- Deprecated Symbols
-  mbuf_is_traffic_class_privileged Deprecated

Function

# mbuf_is_traffic_class_privileged

macOS 10.4–10.15.4Deprecated

``` source
int mbuf_is_traffic_class_privileged(mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf to retrieve the status from.

## Return Value

Non-zero if privileged, 0 otherwise.

## Discussion

Returns the privileged status of the traffic class of the packet specified by the mbuf.

