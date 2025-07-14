

- Hypervisor
-  hv_vcpus_exit(\_:\_:) 

Function

# hv_vcpus_exit(\_:\_:)

Forces an immediate exit of a set of vCPUs of the VM.

macOS 11.0+

``` source
func hv_vcpus_exit(
    _ vcpus: UnsafeMutablePointer,
    _ vcpu_count: UInt32
) -> hv_return_t
```

## Parameters 

`vcpus`  

An array of vCPU instances.

`vcpu_count`  

The number of vCPUs in the array.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## See Also

### Runtime

func hv_vcpu_run(hv_vcpuid_t) -> hv_return_t

Starts the execution of a vCPU.

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

