

- Hypervisor
-  hv_vcpu_set_pending_interrupt(\_:\_:\_:) 

Function

# hv_vcpu_set_pending_interrupt(\_:\_:\_:)

Sets pending interrupts for a vCPU.

macOS 11.0+

``` source
func hv_vcpu_set_pending_interrupt(
    _ vcpu: hv_vcpu_t,
    _ type: hv_interrupt_type_t,
    _ pending: Bool
) -> hv_return_t
```

## Parameters 

`vcpu`  

The instance of the vCPU.

`type`  

The interrupt from `Interrupt Constants`.

`pending`  

A Boolean that indicates whether the interrupt is pending.

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

func hv_vcpu_get_exec_time(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the cumulative execution time of a vCPU, in nanoseconds.

struct hv_interrupt_type_t

The type that defines the vCPU’s interrupts.

Exits

Describe virtual machine exit conditions.

