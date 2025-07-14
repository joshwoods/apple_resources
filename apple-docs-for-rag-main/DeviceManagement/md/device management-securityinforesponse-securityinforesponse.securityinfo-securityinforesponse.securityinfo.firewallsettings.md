

- Device Management
- SecurityInfoResponse
- SecurityInfoResponse.SecurityInfo
-  SecurityInfoResponse.SecurityInfo.FirewallSettings 

Device Management Command

# SecurityInfoResponse.SecurityInfo.FirewallSettings

A dictionary that contains the firewall settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SecurityInfoResponse.SecurityInfo.FirewallSettings
```

## Properties

`Applications`

`[`SecurityInfoResponse.SecurityInfo.FirewallSettings.ApplicationsItem`]`

An array of dictionaries that describes the allowed applications.

`BlockAllIncoming`

`boolean`

If `true`, the firewall blocks all incoming connections.

`FirewallEnabled`

`boolean`

If `true`, the firewall is on.

`LoggingEnabled`

`boolean`

If `true`, logging is enabled.

`LoggingOption`

`string`

The type of logging emitted by the firewall.

Possible Values: `throttled, brief, detail`

`StealthMode`

`boolean`

If true, stealth mode is active for the firewall.

## Discussion

This dictionary is available in macOS 10.12 and later.

## Topics

### Commands

object SecurityInfoResponse.SecurityInfo.FirewallSettings.ApplicationsItem

A dictionary that describes the allowed apps.

## See Also

### Commands

object SecurityInfoResponse.SecurityInfo.FirmwarePasswordStatus

A dictionary that contains the status of the EFI firmware password.

object SecurityInfoResponse.SecurityInfo.ManagementStatus

A dictionary that contains the status of the device’s MDM enrollment.

object SecurityInfoResponse.SecurityInfo.SecureBoot

The response object for the secure boot settings.

object SecurityInfoResponse.SecurityInfo.SecureBoot.ReducedSecurity

A dictionary that contains the device’s reduced security settings.

