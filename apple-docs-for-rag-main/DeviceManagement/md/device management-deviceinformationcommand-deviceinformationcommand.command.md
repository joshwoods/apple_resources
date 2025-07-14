

- Device Management
- DeviceInformationCommand
-  DeviceInformationCommand.Command 

Device Management Command

# DeviceInformationCommand.Command

The request dictionary to query a device for specific information.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeviceInformationCommand.Command
```

## Properties

`Queries`

`[`DeviceInformationCommand.Command.Queries`]`

 (Required) 

An array of query dictionaries to get information about a device.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to query a device for specific information.

Value: `DeviceInformation`

`DeviceAttestationNonce`

`data`

This value can contain up to 32 bytes of data. If specified, queries need to contain `DevicePropertiesAttestation`. If omitted or if the value matches the cached attestation, the system returns the cached attestation. Otherwise, the system requests and returns a new attestation that contains the new nonce.

The nonce appears in the resulting attestation to ensure it was recently generated. To request a new attestation, provide a new nonce. The system caches the most recently generated attestation on the device. Requests for new attestations are rate limited. If it has been fewer than 7 days since the system generated an attestation, the device returns the cached attestation rather than generating a new one.

## Topics

### Commands

object DeviceInformationCommand.Command.Queries

A query dictionary to get information about a device.

