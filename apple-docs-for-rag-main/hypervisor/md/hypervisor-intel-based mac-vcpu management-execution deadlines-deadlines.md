

- Hypervisor
- Intel-based Mac
- vCPU Management
-  Execution Deadlines 

API Collection

# Execution Deadlines

An enumeration that describes available execution deadlines available to vCPUs.

## Topics

### Deadlines

var HV_DEADLINE_FOREVER: UInt

The value that indicates a vCPU deadline that never expires.

## See Also

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

