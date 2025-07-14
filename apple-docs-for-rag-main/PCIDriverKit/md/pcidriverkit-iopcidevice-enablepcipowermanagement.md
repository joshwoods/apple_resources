

- PCIDriverKit
- IOPCIDevice
-  EnablePCIPowerManagement 

Instance Method

# EnablePCIPowerManagement

Configures the device’s PCI bus power management capabilities.

DriverKitmacOS

``` source
kern_return_t EnablePCIPowerManagement(uint64_t state);
```

## Return Value

kIOReturnSuccess if the specified state is supported, or another value if isn’t supported. See Error Codes.

## Discussion

- state: The flags for the power management capabilities you want to enable. If you specify `0xffffffff`, this method lets the IOPCIDevice object determine the desired state. Specify kPCIPMCSPowerStateD0 to disable PCI power management. For a list of possible flags, see Power Management Capabilities.

## See Also

### Managing Power

HasPCIPowerManagement

Determines whether the device has the specified PCI bus power management capabilities.

Power Management Capabilities

Constants you use to get and set the state of the device’s power management features.

Power Management Control/Status Register

Constants you use when checking bits in the power management register.

