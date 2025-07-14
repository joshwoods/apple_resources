

- Hypervisor
- hv_vcpu_exit_exception_t
-  physical_address 

Instance Property

# physical_address

The intermediate physical address of the exception in the client.

macOS

``` source
var physical_address: hv_ipa_t
```

## See Also

### Instance Properties

var syndrome: hv_exception_syndrome_t

The vCPU exception syndrome causing the exception.

var virtual_address: hv_exception_address_t

The vCPU virtual address of the exception.

