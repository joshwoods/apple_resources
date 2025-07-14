

- DriverKit
- IOService
-  ChangePowerState 

Instance Method

# ChangePowerState

Changes the device’s power state to the specified level.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t ChangePowerState(uint32_t powerFlags);
```

## Parameters 

`powerFlags`  

The new power state for the device. Typically, you specify only kIOServicePowerCapabilityLow for this parameter. For a list of all possible values, see Service Power Capabilities.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If the new state is different than the device’s current state, this method places an asynchronous request to change the state to the new value. If the change is successful, the system subsequently calls the SetPowerState method of your service.

## See Also

### Responding to Power-Level Changes

SetPowerState

Updates the service in response to power-related changes for a provider.

Service Power Capabilities

Constants that indicate the power state of a device.

