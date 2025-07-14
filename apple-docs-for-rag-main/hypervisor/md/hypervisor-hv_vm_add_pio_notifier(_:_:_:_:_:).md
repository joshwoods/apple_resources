

- Hypervisor
-  hv_vm_add_pio_notifier(\_:\_:\_:\_:\_:) 

Function

# hv_vm_add_pio_notifier(\_:\_:\_:\_:\_:)

Generate a notification when the Hypervisor issues a matching guest port I/O.

macOS 11.0+

``` source
func hv_vm_add_pio_notifier(
    _ addr: UInt16,
    _ size: Int,
    _ value: UInt32,
    _ mach_port: mach_port_t,
    _ flags: hv_ion_flags_t
) -> hv_return_t
```

## Parameters 

`addr`  

The port I/O address to match.

`size`  

Size to match (1, 2, or 4).

`value`  

The value to match against.

`mach_port`  

The Mach port to write to; requires send permission.

`flags`  

Notifier options using hv_ion_flags_t.

## Return Value

`0` on success, or an hv_return_t error code.

## Discussion

The notifier suppresses guest exits caused by the matching I/O and instead sends a hv_ion_message_t message to the Mach port you specify. The Hypervisor framework only permits one notifier per port address.

## See Also

### I/O notifier functions

func hv_vm_remove_pio_notifier(UInt16, Int, UInt32, mach_port_t, hv_ion_flags_t) -> hv_return_t

Removes an existing I/O notifier that matches the specifications you provide.

struct hv_ion_message_t

The structure that describes the Mach message that the Hypervisor sends when an I/O notifier delivers the notifications you request.

typealias hv_ion_flags_t

The bitfield that you use to set the options flags for the I/O notifier.

I/O Notifier Flags

Flags that you set to choose the kind of information the I/O Notifier delivers.

