

- Hypervisor
-  hv_vcpu_exit_t 

Structure

# hv_vcpu_exit_t

Information about an exit from the vCPU to the host.

macOS

``` source
struct hv_vcpu_exit_t
```

## Topics

### Instance Properties

var exception: hv_vcpu_exit_exception_t

Information about an exit exception from the vcpu to the host.

var reason: hv_exit_reason_t

Information about an exit from the vcpu to the host.

### Initializers

init()

Creates a new exit reason structure.

init(reason: hv_exit_reason_t, exception: hv_vcpu_exit_exception_t)

Creates a new virtual cpu exit structure with a reason and exception that you provide.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

