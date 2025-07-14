

- PCIDriverKit
- IOPCIDevice
-  HasPCIPowerManagement 

Instance Method

# HasPCIPowerManagement

Determines whether the device has the specified PCI bus power management capabilities.

DriverKitmacOS

``` source
kern_return_t HasPCIPowerManagement(uint64_t state);
```

## Return Value

kIOReturnSuccess if the specified state is supported, or another value if isn’t supported. See Error Codes.

## Discussion

- state: The flags for the power management capabilities you want to check. If you specify `0`, this method checks for the power-management information in the device’s registry. For a list of possible flags, see Power Management Capabilities.

## See Also

### Managing Power

EnablePCIPowerManagement

Configures the device’s PCI bus power management capabilities.

Power Management Capabilities

Constants you use to get and set the state of the device’s power management features.

Power Management Control/Status Register

Constants you use when checking bits in the power management register.

