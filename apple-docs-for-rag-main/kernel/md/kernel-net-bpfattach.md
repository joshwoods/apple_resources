

- Kernel
- net
-  bpfattach 

Function

# bpfattach

macOS 10.4+

``` source
void bpfattach(ifnet_t interface, u_int data_link_type, u_int header_length);
```

## Parameters 

`interface`  

The interface to register with BPF.

`data_link_type`  

The data link type of the interface. See the DLT\_\* defines in bpf.h.

`header_length`  

The length, in bytes, of the data link header.

## Discussion

Registers an interface with BPF. This allows bpf devices to attach to your interface to capture packets. Your interface will be unregistered automatically when your interface is detached.

## See Also

### bpf

bpf_attach

bpf_tap_in

bpf_tap_out

