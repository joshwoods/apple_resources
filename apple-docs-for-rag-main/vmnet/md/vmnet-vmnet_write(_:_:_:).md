

- vmnet
-  vmnet_write(\_:\_:\_:) 

Function

# vmnet_write(\_:\_:\_:)

Attempts to write specified packets to an interface.

Mac Catalyst 13.0+macOS 10.10+

``` source
func vmnet_write(
    _ interface: interface_ref,
    _ packets: UnsafeMutablePointer,
    _ pktcnt: UnsafeMutablePointer
) -> vmnet_return_t
```

## Parameters 

`interface`  

The interface reference.

`packets`  

An array of packets to be written.

`pktcnt`  

The number of packets to write. On return, this parameter is populated with the number of packets written.

## Return Value

Returns `vmnet` on success, or an error code on failure. See `vmnet` for possible values.

## Discussion

None of the packet to be written should exceed the size of the value of vmnet_max_packet_size_key for the interface.

## See Also

### Reading and Writing Packets

func vmnet_read(interface_ref, UnsafeMutablePointer&lt;vmpktdesc>, UnsafeMutablePointer&lt;Int32>) -> vmnet_return_t

Attempts to read a specified number of packets from an interface.

