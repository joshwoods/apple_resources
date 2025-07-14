

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
-  MatterAddDeviceExtensionRequestHandler.DeviceCredential 

Structure

# MatterAddDeviceExtensionRequestHandler.DeviceCredential

A collection of device credentials the device presents during commissioning.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
struct DeviceCredential
```

## Topics

### Creating the credential

init(certificationDeclaration: Data, deviceAttestationCertificate: Data, productAttestationIntermediateCertificate: Data)

Creates the credential object.

### Getting the properties

var certificationDeclaration: Data

The device’s Certification Declaration as defined in the Matter specification.

var deviceAttestationCertificate: Data

The device’s Device Attestation Certificate as defined in the Matter specification.

var productAttestationIntermediateCertificate: Data

The device’s Product Attestation Intermediate Certificate as defined in the Matter specification.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Configuring and validating the device

func configureDevice(named: String, in: MatterAddDeviceRequest.Room?) async

Configures the device with selected attributes.

func validateDeviceCredential(MatterAddDeviceExtensionRequestHandler.DeviceCredential) async throws

Performs verification and attestation checks.

func rooms(in: MatterAddDeviceRequest.Home?) async -> [MatterAddDeviceRequest.Room]

Provides rooms that correspond to a home in the device setup.

