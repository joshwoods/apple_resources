

- Device Management
- CertificateListCommand
-  CertificateListCommand.Command 

Device Management Command

# CertificateListCommand.Command

The request dictionary to get a list of installed certificates on a device.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object CertificateListCommand.Command
```

## Properties

`ManagedOnly`

`boolean`

If `true`, only include certificates that MDM installed or that are in the same profile as the MDM payload. User-enrolled devices ignore this value and always only include managed certificates. This value is available in iOS 13 and later, macOS 10.15 and later, and tvOS 13 and later.

Default: `false`

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get a list of installed certificates on a device.

Value: `CertificateList`

