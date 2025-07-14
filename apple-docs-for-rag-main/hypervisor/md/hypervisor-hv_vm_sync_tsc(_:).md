

- Hypervisor
-  hv_vm_sync_tsc(\_:) 

Function

# hv_vm_sync_tsc(\_:)

Synchronizes guest timestamp counters (TSC) across all vCPUs.

macOS 10.10+

``` source
func hv_vm_sync_tsc(_ tsc: UInt64) -> hv_return_t
```

## Parameters 

`tsc`  

The value of the guest TSC.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

