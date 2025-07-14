

- vmnet
-  vmnet_read(\_:\_:\_:) 

Function

# vmnet_read(\_:\_:\_:)

Attempts to read a specified number of packets from an interface.

Mac Catalyst 13.0+macOS 10.10+

``` source
func vmnet_read(
    _ interface: interface_ref,
    _ packets: UnsafeMutablePointer,
    _ pktcnt: UnsafeMutablePointer
) -> vmnet_return_t
```

## Parameters 

`interface`  

The interface reference.

`packets`  

On return, this parameter is populated with an array of packets read.

`pktcnt`  

The number of packets to read. On return, this parameter is populated with the number of packets read, or `0` no packets are available to be read.

## Return Value

Returns `vmnet` on success, or an error code on failure. See `vmnet` for possible values.

## Discussion

Each packet buffer passed should be at least as large as the value of vmnet_max_packet_size_key for the interface.

## See Also

### Reading and Writing Packets

func vmnet_write(interface_ref, UnsafeMutablePointer&lt;vmpktdesc>, UnsafeMutablePointer&lt;Int32>) -> vmnet_return_t

Attempts to write specified packets to an interface.

