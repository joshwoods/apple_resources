

- Hypervisor
- hv_vcpu_exit_exception_t
-  virtual_address 

Instance Property

# virtual_address

The vCPU virtual address of the exception.

macOS

``` source
var virtual_address: hv_exception_address_t
```

## See Also

### Instance Properties

var physical_address: hv_ipa_t

The intermediate physical address of the exception in the client.

var syndrome: hv_exception_syndrome_t

The vCPU exception syndrome causing the exception.

