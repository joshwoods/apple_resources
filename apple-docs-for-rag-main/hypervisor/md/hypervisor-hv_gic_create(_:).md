

- Hypervisor
-  hv_gic_create(\_:) 

Function

# hv_gic_create(\_:)

Creates a generic interrupt controller (GIC) v3 device for a VM configuration.

macOS 15.0+

``` source
func hv_gic_create(_ gic_config: hv_gic_config_t) -> hv_return_t
```

## Parameters 

`gic_config`  

A GIC configuration object.

## Return Value

HV_SUCCESS on success, an error code otherwise.

## Discussion

Important

Only call this method after a virtual machine (VM) has started, but before you create vCPUs so that the framework can allocate GIC CPU system resources. If either of these conditions aren’t met, the framework returns an error.

Use this method to create an ARM Generic Interrupt Controller (GIC) v3 device. The framework supports a maximum of one instance of this device per VM. The device supports a distributor, redistributors, MSIs, and GIC CPU system registers.

When EL2 is enabled, the device supports GIC hypervisor control registers which the guest hypervisor uses to inject interrupts to its guest. The framework doesn’t support the Hypervisor’s vCPU get or set interrupt functions for injecting interrupts to a nested guest.

GIC v3 uses affinity based interrupt routing. vCPUs must set affinity values in their `MPIDR_EL1` register. When the virtual machine vCPUs are running, the framework considers its topology final. Destroy vCPUs only when you’re tearing down the virtual machine.

Hypervisor only provides GIC MSI support when you’ve both configured an MSI region base address and set an MSI interrupt range.

