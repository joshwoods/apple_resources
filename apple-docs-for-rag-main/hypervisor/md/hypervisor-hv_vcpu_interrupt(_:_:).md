

- Hypervisor
-  hv_vcpu_interrupt(\_:\_:) 

Function

# hv_vcpu_interrupt(\_:\_:)

Forces the vCPU instances you provide to immediately exit the VM.

macOS 10.10+

``` source
func hv_vcpu_interrupt(
    _ vcpus: UnsafeMutablePointer,
    _ vcpu_count: UInt32
) -> hv_return_t
```

## Parameters 

`vcpus`  

A pointer to an array of instances of vCPU.

`vcpu_count`  

The number of vCPU IDs specified by `vcpus`.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## See Also

### Runtime

func hv_vcpu_run_until(hv_vcpuid_t, UInt64) -> hv_return_t

Executes a vCPU until it reaches the deadline defined in absolute time units you provide.

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

