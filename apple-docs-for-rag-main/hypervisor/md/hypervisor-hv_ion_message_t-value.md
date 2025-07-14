

- Hypervisor
- hv_ion_message_t
-  value 

Instance Property

# value

An unsigned 64-bit integer that represents the contents of an I/O notifier message.

macOS

``` source
var value: UInt64
```

## See Also

### Instance properties

var addr: UInt64

The address of the I/O write.

var header: mach_msg_header_t

The Mach message header.

var size: UInt64

The size of the value written by the notifier.

var trailer: mach_msg_trailer_t

The Mach message trailer.

