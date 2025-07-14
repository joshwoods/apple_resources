

- Kernel
- Kernel Data Types
-  bpf_packet_func 

Type Alias

# bpf_packet_func

macOS 10.4+

``` source
typedef errno_t (*bpf_packet_func)(ifnet_t interface, mbuf_t data);
```

## Parameters 

`interface`  

The interface being sent or received on.

`data`  

The packet to be transmitted or received.

## Return Value

An errno value or zero upon success.

## Discussion

bpf_packet_func The bpf_packet_func is used to intercept inbound and outbound packets. The tap function will never free the mbuf. The tap function will only copy the mbuf in to various bpf file descriptors tapping this interface.

