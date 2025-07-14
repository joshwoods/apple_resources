

- Hypervisor
- hv_vcpu_exit_exception_t
-  init() 

Initializer

# init()

Creates a new VCPU exit exception instance.

macOS

``` source
init()
```

## See Also

### Initializers

init(syndrome: hv_exception_syndrome_t, virtual_address: hv_exception_address_t, physical_address: hv_ipa_t)

Creates a new VCPU exit exception instance.with the parameters you provide.

