

- Hypervisor
-  hv_vcpu_run(\_:) 

Function

# hv_vcpu_run(\_:)

Starts the execution of a vCPU.

macOS

``` source
func hv_vcpu_run(_ vcpu: hv_vcpuid_t) -> hv_return_t
```

## Parameters 

`vcpu`  

The instance of the vCPU.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Call blocks until the next exit of the vCPU. The owning thread must call this function.

On an Apple Silicon, if the exit is of type HV_EXIT_REASON_VTIMER_ACTIVATED, the VTimer is automatically masked. As a result, no timer fires until the timer is unmasked with hv_vcpu_set_vtimer_mask(_:_:).

On an Intel-based Mac, hv_vcpu_run(_:) exits from causes external to the guest. To avoid the overhead of spurious exits use hv_vcpu_run_until(_:_:) with the deadline HV_DEADLINE_FOREVER.

## See Also

### Runtime

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

Exits

Describe virtual machine exit conditions.

