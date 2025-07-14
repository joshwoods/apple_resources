

- Hypervisor
- hv_vcpu_exit_exception_t
-  syndrome 

Instance Property

# syndrome

The vCPU exception syndrome causing the exception.

macOS

``` source
var syndrome: hv_exception_syndrome_t
```

## See Also

### Instance Properties

var physical_address: hv_ipa_t

The intermediate physical address of the exception in the client.

var virtual_address: hv_exception_address_t

The vCPU virtual address of the exception.

