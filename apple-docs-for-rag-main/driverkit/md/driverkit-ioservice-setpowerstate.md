

- DriverKit
- IOService
-  SetPowerState 

Instance Method

# SetPowerState

Updates the service in response to power-related changes for a provider.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetPowerState(uint32_t powerFlags);
```

## Parameters 

`powerFlags`  

The new power state for the service’s provider object. Configure your driver appropriately for the new state. For a list of possible values, see Service Power Capabilities.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

DriverKit calls this method to notify your service when the power state of its provider changes. Implement this method in your service object and use it to put your driver in a safe state for the new power setting. Call `super` as the last step in your implementation.

## See Also

### Responding to Power-Level Changes

ChangePowerState

Changes the device’s power state to the specified level.

Service Power Capabilities

Constants that indicate the power state of a device.

