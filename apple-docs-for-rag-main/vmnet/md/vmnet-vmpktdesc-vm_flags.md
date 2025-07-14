

- vmnet
- vmpktdesc
-  vm_flags 

Instance Property

# vm_flags

Option flags. Should be set to `0` on read.

Mac Catalyst 13.0+macOS 10.10+

``` source
var vm_flags: UInt32
```

## See Also

### Fields

var vm_pkt_iov: UnsafeMutablePointer&lt;iovec>

An array of packet buffers.

var vm_pkt_iovcnt: UInt32

The number of packet buffers in `vm_pkt_iov`.

var vm_pkt_size: Int

The size of the packet, in bytes.

