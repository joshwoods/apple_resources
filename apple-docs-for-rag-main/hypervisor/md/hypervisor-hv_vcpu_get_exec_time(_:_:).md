

- Hypervisor
-  hv_vcpu_get_exec_time(\_:\_:) 

Function

# hv_vcpu_get_exec_time(\_:\_:)

Returns, by reference, the cumulative execution time of a vCPU, in nanoseconds.

macOS 10.10+

``` source
func hv_vcpu_get_exec_time(
    _ vcpu: hv_vcpuid_t,
    _ time: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`vcpu`  

The instance of the vCPU.

`time`  

The execution time on output, in nanoseconds.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Important

This function must be called by the owning thread.

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

struct hv_interrupt_type_t

The type that defines the vCPU’s interrupts.

Exits

Describe virtual machine exit conditions.

