

- Hypervisor
- Apple Silicon
- vCPU Management
-  Exits 

API Collection

# Exits

Describe virtual machine exit conditions.

## Topics

### Descriptor

struct hv_vcpu_exit_t

Information about an exit from the vCPU to the host.

### Exit reasons

struct hv_exit_reason_t

The type that describes the event that triggered a guest exit to the host.

typealias hv_exception_syndrome_t

Type of a vCPU exception syndrome.

typealias hv_exception_address_t

Type of a vCPU exception virtual address.

## See Also

### Runtime

func hv_vcpu_run(hv_vcpuid_t) -> hv_return_t

Starts the execution of a vCPU.

func hv_vcpus_exit(UnsafeMutablePointer&lt;hv_vcpu_t>, UInt32) -> hv_return_t

Forces an immediate exit of a set of vCPUs of the VM.

func hv_vcpu_get_pending_interrupt(hv_vcpu_t, hv_interrupt_type_t, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

Gets pending interrupts for a vCPU.

func hv_vcpu_set_pending_interrupt(hv_vcpu_t, hv_interrupt_type_t, Bool) -> hv_return_t

Sets pending interrupts for a vCPU.

func hv_vcpu_get_exec_time(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the cumulative execution time of a vCPU, in nanoseconds.

struct hv_interrupt_type_t

The type that defines the vCPU’s interrupts.

