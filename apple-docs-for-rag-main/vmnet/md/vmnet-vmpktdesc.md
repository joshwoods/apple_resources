

- vmnet
-  vmpktdesc 

Structure

# vmpktdesc

Describes a packet.

Mac Catalyst 13.0+macOS 10.10+

``` source
struct vmpktdesc
```

## Topics

### Fields

var vm_flags: UInt32

Option flags. Should be set to `0` on read.

var vm_pkt_iov: UnsafeMutablePointer&lt;iovec>

An array of packet buffers.

var vm_pkt_iovcnt: UInt32

The number of packet buffers in `vm_pkt_iov`.

var vm_pkt_size: Int

The size of the packet, in bytes.

### Initializers

init(vm_pkt_size: Int, vm_pkt_iov: UnsafeMutablePointer&lt;iovec>, vm_pkt_iovcnt: UInt32, vm_flags: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

enum vmnet_return_t

Values returned by functions in the vmnet Framework.

typealias interface_ref

A virtual network interface.

struct interface_event_t

Interface event types.

enum operating_modes_t

The operating modes for an interface.

