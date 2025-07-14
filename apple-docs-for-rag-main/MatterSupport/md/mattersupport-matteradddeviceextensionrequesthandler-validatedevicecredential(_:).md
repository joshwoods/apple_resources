

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
-  validateDeviceCredential(\_:) 

Instance Method

# validateDeviceCredential(\_:)

Performs verification and attestation checks.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
func validateDeviceCredential(_ deviceCredential: MatterAddDeviceExtensionRequestHandler.DeviceCredential) async throws
```

## Overview

Override this method to perform additional verification and attestation checks, which execute after Apple’s built-in device attestation checks. If either attestation fails as indicated by an exception thrown here, a warning dialog appears before proceeding.

This is the first callback that the system invokes during the setup flow. It runs after selecting a device but before commissioning, and can abort commissioning if the credential is rejected by throwing an exception.

## See Also

### Configuring and validating the device

func configureDevice(named: String, in: MatterAddDeviceRequest.Room?) async

Configures the device with selected attributes.

struct DeviceCredential

A collection of device credentials the device presents during commissioning.

func rooms(in: MatterAddDeviceRequest.Home?) async -> [MatterAddDeviceRequest.Room]

Provides rooms that correspond to a home in the device setup.

