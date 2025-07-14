

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
-  configureDevice(named:in:) 

Instance Method

# configureDevice(named:in:)

Configures the device with selected attributes.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
func configureDevice(
    named name: String,
    in room: MatterAddDeviceRequest.Room?
) async
```

## Parameters 

`name`  

The selected name for the device.

`room`  

The selected room for the device.

## See Also

### Configuring and validating the device

func validateDeviceCredential(MatterAddDeviceExtensionRequestHandler.DeviceCredential) async throws

Performs verification and attestation checks.

struct DeviceCredential

A collection of device credentials the device presents during commissioning.

func rooms(in: MatterAddDeviceRequest.Home?) async -> [MatterAddDeviceRequest.Room]

Provides rooms that correspond to a home in the device setup.

