

- vmnet
- vmpktdesc
-  vm_pkt_size 

Instance Property

# vm_pkt_size

The size of the packet, in bytes.

Mac Catalyst 13.0+macOS 10.10+

``` source
var vm_pkt_size: Int
```

## See Also

### Fields

var vm_flags: UInt32

Option flags. Should be set to `0` on read.

var vm_pkt_iov: UnsafeMutablePointer&lt;iovec>

An array of packet buffers.

var vm_pkt_iovcnt: UInt32

The number of packet buffers in `vm_pkt_iov`.

