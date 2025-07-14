

- Hypervisor
- hv_ion_message_t
-  addr 

Instance Property

# addr

The address of the I/O write.

macOS

``` source
var addr: UInt64
```

## See Also

### Instance properties

var header: mach_msg_header_t

The Mach message header.

var size: UInt64

The size of the value written by the notifier.

var trailer: mach_msg_trailer_t

The Mach message trailer.

var value: UInt64

An unsigned 64-bit integer that represents the contents of an I/O notifier message.

