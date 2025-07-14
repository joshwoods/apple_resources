

- Hypervisor
- Intel-based Mac
-  vCPU Management 

API Collection

# vCPU Management

Create and run virtual CPUs, and manage CPU-specific registers and features.

## Topics

### Creation and destruction

func hv_vcpu_create(UnsafeMutablePointer&lt;hv_vcpuid_t>, hv_vcpu_options_t) -> hv_return_t

Creates a vCPU instance for the current thread.

func hv_vcpu_destroy(hv_vcpuid_t) -> hv_return_t

Destroys the vCPU instance associated with the current thread.

typealias hv_vcpu_options_t

Options for creating a new vCPU instance.

vCPU Creation Behavior

An enumeration representing the default creation options for virtual CPUs.

typealias hv_vcpuid_t

The type that describes a vCPU ID.

### Runtime

func hv_vcpu_run_until(hv_vcpuid_t, UInt64) -> hv_return_t

Executes a vCPU until it reaches the deadline defined in absolute time units you provide.

func hv_vcpu_interrupt(UnsafeMutablePointer&lt;hv_vcpuid_t>, UInt32) -> hv_return_t

Forces the vCPU instances you provide to immediately exit the VM.

func hv_vcpu_invalidate_tlb(hv_vcpuid_t) -> hv_return_t

Invalidates the translation look-aside buffer (TLB) of a vCPU.

func hv_vcpu_flush(hv_vcpuid_t) -> hv_return_t

Flushes the cached state of a vCPU.

Deprecated

func hv_vcpu_get_exec_time(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the cumulative execution time of a vCPU, in nanoseconds.

func hv_vcpu_run(hv_vcpuid_t) -> hv_return_t

Starts the execution of a vCPU.

Execution Deadlines

An enumeration that describes available execution deadlines available to vCPUs.

### Synchronization

func hv_vm_sync_tsc(UInt64) -> hv_return_t

Synchronizes guest timestamp counters (TSC) across all vCPUs.

### Model-Specific Registers

Extending vCPU Capabilities Using Model-Specific Registers

Configure specific client performance monitoring and enable other vCPU capabilities using Model-Specific Registers.

func hv_vcpu_read_msr(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the current value of a Model-Specific Register (MSR) of a vCPU.

func hv_vcpu_write_msr(hv_vcpuid_t, UInt32, UInt64) -> hv_return_t

Sets the value of a Model-Specific Register (MSR) of a vCPU.

func hv_vcpu_enable_native_msr(hv_vcpuid_t, UInt32, Bool) -> hv_return_t

Enables or disables a Model-Specific Register (MSR) that the VM uses natively.

func hv_vcpu_set_msr_access(hv_vcpuid_t, UInt32, hv_msr_flags_t) -> hv_return_t

Controls the guest access of a managed Model-Specific Register (MSR).

func hv_vcpu_enable_managed_msr(hv_vcpuid_t, UInt32, Bool) -> hv_return_t

Enables the guest access of a managed Model-Specific Register (MSR).

typealias hv_msr_flags_t

The type representing the native Model-Specific Register (MSR) permissions.

Model-Specific Registers

MSR Permissions

An enumeration that describes possible Model-Specific Register (MSR) permisssions.

### CPU Registers

func hv_vcpu_read_register(hv_vcpuid_t, hv_x86_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the current value of an architectural x86 register of a vCPU.

func hv_vcpu_write_register(hv_vcpuid_t, hv_x86_reg_t, UInt64) -> hv_return_t

Sets the value of an architectural x86 register of a vCPU.

struct hv_x86_reg_t

The type that defines x86 architectural registers.

### Floating Point (FP) State

func hv_vcpu_read_fpstate(hv_vcpuid_t, UnsafeMutableRawPointer, Int) -> hv_return_t

Returns, by reference, the current architectural x86 floating point and SIMD state of a vCPU.

func hv_vcpu_write_fpstate(hv_vcpuid_t, UnsafeMutableRawPointer, Int) -> hv_return_t

Sets the architectural x86 floating point and SIMD state of a vCPU.

### Memory Affinity

func hv_vcpu_set_space(hv_vcpuid_t, hv_vm_space_t) -> hv_return_t

Associates the vCPU instance with an allocated address space.

## See Also

### Resource management

Memory Management

Map memory into the physical address space of the virtual machine, and allocate additional memory for the current task.

Virtual Machine Control Structure (VMCS)

Read and write to fields of the virtual machine control structure.

