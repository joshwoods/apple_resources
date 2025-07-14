

- Hypervisor
-  hv_vm_remove_pio_notifier(\_:\_:\_:\_:\_:) 

Function

# hv_vm_remove_pio_notifier(\_:\_:\_:\_:\_:)

Removes an existing I/O notifier that matches the specifications you provide.

macOS 11.0+

``` source
func hv_vm_remove_pio_notifier(
    _ addr: UInt16,
    _ size: Int,
    _ value: UInt32,
    _ mach_port: mach_port_t,
    _ flags: hv_ion_flags_t
) -> hv_return_t
```

## Parameters 

`addr`  

The port I/O address of the existing notifier.

`size`  

The match-size from the existing notifier.

`value`  

The value to match against from the existing notifier.

`mach_port`  

The Mach port from the existing notifier.

`flags`  

The hv_ion_flags_t option flags from the existing notifier.

## Return Value

`0` on success, or an hv_return_t error code.

## Discussion

The arguments you provide must match those previously used to add the notifier.

## See Also

### I/O notifier functions

func hv_vm_add_pio_notifier(UInt16, Int, UInt32, mach_port_t, hv_ion_flags_t) -> hv_return_t

Generate a notification when the Hypervisor issues a matching guest port I/O.

struct hv_ion_message_t

The structure that describes the Mach message that the Hypervisor sends when an I/O notifier delivers the notifications you request.

typealias hv_ion_flags_t

The bitfield that you use to set the options flags for the I/O notifier.

I/O Notifier Flags

Flags that you set to choose the kind of information the I/O Notifier delivers.

