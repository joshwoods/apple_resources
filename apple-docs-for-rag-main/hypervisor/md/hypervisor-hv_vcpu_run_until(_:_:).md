

- Hypervisor
-  hv_vcpu_run_until(\_:\_:) 

Function

# hv_vcpu_run_until(\_:\_:)

Executes a vCPU until it reaches the deadline defined in absolute time units you provide.

macOS 10.15+

``` source
func hv_vcpu_run_until(
    _ vcpu: hv_vcpuid_t,
    _ deadline: UInt64
) -> hv_return_t
```

## Parameters 

`vcpu`  

The instance of the vCPU.

`deadline`  

The timer deadline in mach absolute time units. Use the special value HV_DEADLINE_FOREVER to specify a deadline that never expires.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

If the deadline you specify is other than HV_DEADLINE_FOREVER, this call uses the VMX preemption timer. If the hardware doesn’t support the VMX preemption timer, it returns HV_UNSUPPORTED.

This function supersedes hv_vcpu_run(_:) on Intel-based Mac computers. Unlike hv_vcpu_run(_:), it doesn’t return on transparently handled VMEXITs.

## See Also

### Runtime

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

