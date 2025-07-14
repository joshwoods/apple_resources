

- Device Management
- SecurityInfoResponse
- SecurityInfoResponse.SecurityInfo
-  SecurityInfoResponse.SecurityInfo.SecureBoot 

Device Management Command

# SecurityInfoResponse.SecurityInfo.SecureBoot

The response object for the secure boot settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SecurityInfoResponse.SecurityInfo.SecureBoot
```

## Properties

`ExternalBootLevel`

`string`

The device’s external boot level, which indicates whether it allows booting from an external device, disallows it, or doesn’t support it.

Possible Values: `allowed, disallowed, not supported`

`SecureBootLevel`

`string`

The security level for the bootable operating system versions.

Possible Values: `off, medium, full, not supported`

`ReducedSecurity`

`[`SecurityInfoResponse.SecurityInfo.SecureBoot.ReducedSecurity`]`

Reports which security features the user disables in `recoveryOS`. This property is only present for Apple silicon when `SecureBootLevel` is `medium`.

Available in iOS 11 and later.

## Discussion

This dictionary is available in macOS 10.15 and later.

## Topics

### Commands

object SecurityInfoResponse.SecurityInfo.SecureBoot.ReducedSecurity

A dictionary that contains the device’s reduced security settings.

## See Also

### Commands

object SecurityInfoResponse.SecurityInfo.FirewallSettings

A dictionary that contains the firewall settings.

object SecurityInfoResponse.SecurityInfo.FirmwarePasswordStatus

A dictionary that contains the status of the EFI firmware password.

object SecurityInfoResponse.SecurityInfo.ManagementStatus

A dictionary that contains the status of the device’s MDM enrollment.

object SecurityInfoResponse.SecurityInfo.SecureBoot.ReducedSecurity

A dictionary that contains the device’s reduced security settings.

