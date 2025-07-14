

- Kernel
- net
-  bpf_tap_in 

Function

# bpf_tap_in

macOS 10.5+

``` source
void bpf_tap_in(ifnet_t interface, u_int32_t dlt, mbuf_t packet, void *header, size_t header_len);
```

## Parameters 

`interface`  

The interface the packet was received on.

`dlt`  

The data link type of the packet.

`packet`  

The packet received.

`header`  

An optional pointer to a header that will be prepended.

`headerlen`  

If the header was specified, the length of the header.

## Discussion

Call this function when your interface receives a packet. This function will check if any bpf devices need a a copy of the packet.

## See Also

### bpf

bpf_attach

bpf_tap_out

bpfattach

