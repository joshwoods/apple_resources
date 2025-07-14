

- Hypervisor
- Intel-based Mac
-  I/O Notifier Flags 

API Collection

# I/O Notifier Flags

Flags that you set to choose the kind of information the I/O Notifier delivers.

## Topics

### Notifier options

var HV_ION_ANY_SIZE: Int

The value that represents a request for notifications of an I/O result of any size.

var HV_ION_ANY_VALUE: Int

The value that represents a request for notifications of an I/O result that contains any value.

var HV_ION_EXIT_FULL: Int

The value that represents a request for notifications if the I/O queue is full.

var HV_ION_NONE: Int

The value that represents a request for no notifications.

## See Also

### I/O notifier functions

func hv_vm_add_pio_notifier(UInt16, Int, UInt32, mach_port_t, hv_ion_flags_t) -> hv_return_t

Generate a notification when the Hypervisor issues a matching guest port I/O.

func hv_vm_remove_pio_notifier(UInt16, Int, UInt32, mach_port_t, hv_ion_flags_t) -> hv_return_t

Removes an existing I/O notifier that matches the specifications you provide.

struct hv_ion_message_t

The structure that describes the Mach message that the Hypervisor sends when an I/O notifier delivers the notifications you request.

typealias hv_ion_flags_t

The bitfield that you use to set the options flags for the I/O notifier.

