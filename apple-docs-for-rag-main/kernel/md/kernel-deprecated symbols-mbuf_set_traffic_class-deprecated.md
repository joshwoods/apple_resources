

- Kernel
- Deprecated Symbols
-  mbuf_set_traffic_class Deprecated

Function

# mbuf_set_traffic_class

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_set_traffic_class(mbuf_t mbuf, mbuf_traffic_class_t tc);
```

## Parameters 

`mbuf`  

The mbuf to set the traffic class on. @tc The traffic class

## Return Value

0 on success, EINVAL if bad parameter is passed

## Discussion

Set the traffic class of an mbuf packet.

