

- DriverKit
- IOService
-  Service Power Capabilities 

API Collection

# Service Power Capabilities

Constants that indicate the power state of a device.

## Topics

### Getting the Power Levels

kIOServicePowerCapabilityOff

The device is entering the sleep state.

kIOServicePowerCapabilityOn

The device is fully powered.

kIOServicePowerCapabilityLow

The device is in a reduced power state, but the system is running.

## See Also

### Responding to Power-Level Changes

SetPowerState

Updates the service in response to power-related changes for a provider.

ChangePowerState

Changes the device’s power state to the specified level.

