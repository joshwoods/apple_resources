

- Kernel
- Deprecated Symbols
-  mbuf_pkthdr_rcvif Deprecated

Function

# mbuf_pkthdr_rcvif

macOS 10.4–10.15.4Deprecated

``` source
ifnet_t mbuf_pkthdr_rcvif(const mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf containing the packet header.

## Return Value

A reference to the interface.

## Discussion

Returns the interface the packet was received on. This funciton does not modify the reference count of the interface. The interface is only valid for as long as the mbuf is not freed and the rcvif for the mbuf is not changed. Take a reference on the interface that you will release later before doing any of the following: free the mbuf, change the rcvif, pass the mbuf to any function that may free the mbuf or change the rcvif.

