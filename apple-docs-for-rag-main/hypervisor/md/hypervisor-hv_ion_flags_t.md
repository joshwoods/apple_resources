

- Hypervisor
-  hv_ion_flags_t 

Type Alias

# hv_ion_flags_t

The bitfield that you use to set the options flags for the I/O notifier.

macOS

``` source
typealias hv_ion_flags_t = UInt32
```

## See Also

### I/O notifier functions

func hv_vm_add_pio_notifier(UInt16, Int, UInt32, mach_port_t, hv_ion_flags_t) -> hv_return_t

Generate a notification when the Hypervisor issues a matching guest port I/O.

func hv_vm_remove_pio_notifier(UInt16, Int, UInt32, mach_port_t, hv_ion_flags_t) -> hv_return_t

Removes an existing I/O notifier that matches the specifications you provide.

struct hv_ion_message_t

The structure that describes the Mach message that the Hypervisor sends when an I/O notifier delivers the notifications you request.

I/O Notifier Flags

Flags that you set to choose the kind of information the I/O Notifier delivers.

