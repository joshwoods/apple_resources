

- Hypervisor
- hv_vcpu_exit_t
-  init(reason:exception:) 

Initializer

# init(reason:exception:)

Creates a new virtual cpu exit structure with a reason and exception that you provide.

macOS

``` source
init(
    reason: hv_exit_reason_t,
    exception: hv_vcpu_exit_exception_t
)
```

## Parameters 

`reason`  

The hv_exit_reason_t result code that describes the reason for the exception.

`exception`  

The exception struture.

## See Also

### Initializers

init()

Creates a new exit reason structure.

