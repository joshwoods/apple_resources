

- Hypervisor
-  HV_VCPU_TSC_RELATIVE 

Global Variable

# HV_VCPU_TSC_RELATIVE

The value that represents the relative offset the system should add to the hypervisor TSC clock.

macOS

``` source
var HV_VCPU_TSC_RELATIVE: Int { get }
```

## See Also

### Constants

var HV_VCPU_DEFAULT: Int

The default vCPU creation behavior.

var HV_VCPU_ACCEL_RDPMC: Int

Instructs the kernel, when set, to handle RDPMC VM exits directly rather than passing them to user space.

