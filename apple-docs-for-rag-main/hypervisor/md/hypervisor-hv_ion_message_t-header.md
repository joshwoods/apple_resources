

- Hypervisor
- hv_ion_message_t
-  header 

Instance Property

# header

The Mach message header.

macOS

``` source
var header: mach_msg_header_t
```

## See Also

### Instance properties

var addr: UInt64

The address of the I/O write.

var size: UInt64

The size of the value written by the notifier.

var trailer: mach_msg_trailer_t

The Mach message trailer.

var value: UInt64

An unsigned 64-bit integer that represents the contents of an I/O notifier message.

