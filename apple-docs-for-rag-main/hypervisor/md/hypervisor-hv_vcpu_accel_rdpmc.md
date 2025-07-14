

- Hypervisor
-  HV_VCPU_ACCEL_RDPMC 

Global Variable

# HV_VCPU_ACCEL_RDPMC

Instructs the kernel, when set, to handle RDPMC VM exits directly rather than passing them to user space.

macOS

``` source
var HV_VCPU_ACCEL_RDPMC: Int { get }
```

## Mentioned in 

Extending vCPU Capabilities Using Model-Specific Registers

## Discussion

When the guest issues RDPMC instructions, a VM exit occurs. When set, this flag instructs the kernel to handle RDRPMC VM exits directly, and more efficiently, than passing them on to user space.

## See Also

### Constants

var HV_VCPU_DEFAULT: Int

The default vCPU creation behavior.

var HV_VCPU_TSC_RELATIVE: Int

The value that represents the relative offset the system should add to the hypervisor TSC clock.

