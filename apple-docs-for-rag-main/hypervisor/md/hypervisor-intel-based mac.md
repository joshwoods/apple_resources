

- Hypervisor
-  Intel-based Mac 

API Collection

# Intel-based Mac

Create and run virtual machines on Intel-based Mac computers.

## Topics

### Virtual machine management

func hv_vm_create(hv_vm_options_t) -> hv_return_t

Creates a VM instance for the current process.

func hv_vm_destroy() -> hv_return_t

Destroys the VM instance associated with the current process.

func hv_capability(hv_capability_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the value of capabilities of the system.

typealias hv_vm_options_t

Options you use when creating a virtual machine.

typealias hv_capability_t

The type of system capabilities.

### Resource management

vCPU Management

Create and run virtual CPUs, and manage CPU-specific registers and features.

Memory Management

Map memory into the physical address space of the virtual machine, and allocate additional memory for the current task.

Virtual Machine Control Structure (VMCS)

Read and write to fields of the virtual machine control structure.

### I/O notifier functions

func hv_vm_add_pio_notifier(UInt16, Int, UInt32, mach_port_t, hv_ion_flags_t) -> hv_return_t

Generate a notification when the Hypervisor issues a matching guest port I/O.

func hv_vm_remove_pio_notifier(UInt16, Int, UInt32, mach_port_t, hv_ion_flags_t) -> hv_return_t

Removes an existing I/O notifier that matches the specifications you provide.

struct hv_ion_message_t

The structure that describes the Mach message that the Hypervisor sends when an I/O notifier delivers the notifications you request.

typealias hv_ion_flags_t

The bitfield that you use to set the options flags for the I/O notifier.

I/O Notifier Flags

Flags that you set to choose the kind of information the I/O Notifier delivers.

### Time-stamp counter functions

func hv_tsc_clock() -> UInt64

Returns the value of an abstract clock.

func hv_vcpu_set_tsc_relative(hv_vcpuid_t, Int64) -> hv_return_t

Sets the offset of the guest timestamp-counter (TSC) relative to the Hypervisor’s TSC clock.

### Common data types

typealias hv_return_t

The return type of framework functions.

Hypervisor Errors

Errors returned by Hypervisor functions.

## See Also

### Platforms

Apple Silicon

Create and run virtual machines on Apple silicon.

