

- Hypervisor
-  hv_exception_address_t 

Type Alias

# hv_exception_address_t

Type of a vCPU exception virtual address.

macOS

``` source
typealias hv_exception_address_t = UInt64
```

## Discussion

This corresponds to Fault Address Register EL2 (FAR_EL2).

## See Also

### Exit reasons

struct hv_exit_reason_t

The type that describes the event that triggered a guest exit to the host.

typealias hv_exception_syndrome_t

Type of a vCPU exception syndrome.

