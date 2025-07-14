

- Hypervisor
-  hv_ion_message_t 

Structure

# hv_ion_message_t

The structure that describes the Mach message that the Hypervisor sends when an I/O notifier delivers the notifications you request.

macOS

``` source
struct hv_ion_message_t
```

## Topics

### Initializers

init()

Creates a new I/O notifier message.

init(header: mach_msg_header_t, addr: UInt64, size: UInt64, value: UInt64, trailer: mach_msg_trailer_t)

Creates a new I/O notifier message with the parameters you provide.

### Instance properties

var addr: UInt64

The address of the I/O write.

var header: mach_msg_header_t

The Mach message header.

var size: UInt64

The size of the value written by the notifier.

var trailer: mach_msg_trailer_t

The Mach message trailer.

var value: UInt64

An unsigned 64-bit integer that represents the contents of an I/O notifier message.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### I/O notifier functions

func hv_vm_add_pio_notifier(UInt16, Int, UInt32, mach_port_t, hv_ion_flags_t) -> hv_return_t

Generate a notification when the Hypervisor issues a matching guest port I/O.

func hv_vm_remove_pio_notifier(UInt16, Int, UInt32, mach_port_t, hv_ion_flags_t) -> hv_return_t

Removes an existing I/O notifier that matches the specifications you provide.

typealias hv_ion_flags_t

The bitfield that you use to set the options flags for the I/O notifier.

I/O Notifier Flags

Flags that you set to choose the kind of information the I/O Notifier delivers.

