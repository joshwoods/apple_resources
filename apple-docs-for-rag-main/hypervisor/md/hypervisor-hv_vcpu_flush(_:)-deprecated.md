

- Hypervisor
-  hv_vcpu_flush(\_:) Deprecated

Function

# hv_vcpu_flush(\_:)

Flushes the cached state of a vCPU.

macOS 10.10–11.0Deprecated

``` source
func hv_vcpu_flush(_ vcpu: hv_vcpuid_t) -> hv_return_t
```

Deprecated

This API has no effect and always returns HV_UNSUPPORTED

## Parameters 

`vcpu`  

The instance of the vCPU.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

This function must be called by the owning thread.

## See Also

### Runtime

func hv_vcpu_run_until(hv_vcpuid_t, UInt64) -> hv_return_t

Executes a vCPU until it reaches the deadline defined in absolute time units you provide.

func hv_vcpu_interrupt(UnsafeMutablePointer&lt;hv_vcpuid_t>, UInt32) -> hv_return_t

Forces the vCPU instances you provide to immediately exit the VM.

func hv_vcpu_invalidate_tlb(hv_vcpuid_t) -> hv_return_t

Invalidates the translation look-aside buffer (TLB) of a vCPU.

func hv_vcpu_get_exec_time(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the cumulative execution time of a vCPU, in nanoseconds.

func hv_vcpu_run(hv_vcpuid_t) -> hv_return_t

Starts the execution of a vCPU.

Execution Deadlines

An enumeration that describes available execution deadlines available to vCPUs.

