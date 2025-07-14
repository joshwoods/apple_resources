

- Device Management
- SecurityInfoResponse
- SecurityInfoResponse.SecurityInfo
-  SecurityInfoResponse.SecurityInfo.FirmwarePasswordStatus 

Device Management Command

# SecurityInfoResponse.SecurityInfo.FirmwarePasswordStatus

A dictionary that contains the status of the EFI firmware password.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SecurityInfoResponse.SecurityInfo.FirmwarePasswordStatus
```

## Properties

`AllowOroms`

`boolean`

If `true`, enable ROMs.

`ChangePending`

`boolean`

If `true`, a firmware password change is pending. A device restart is necessary for this change to take effect. Until then, additional attempts to change the password fail.

Note

If `true`, the other values show the current state of the device, not the state after a restart.

`PasswordExists`

`boolean`

If `true`, the device has an EFI firmware password.

## Discussion

This dictionary is available in macOS 10.13 and later.

## See Also

### Commands

object SecurityInfoResponse.SecurityInfo.FirewallSettings

A dictionary that contains the firewall settings.

object SecurityInfoResponse.SecurityInfo.ManagementStatus

A dictionary that contains the status of the device’s MDM enrollment.

object SecurityInfoResponse.SecurityInfo.SecureBoot

The response object for the secure boot settings.

object SecurityInfoResponse.SecurityInfo.SecureBoot.ReducedSecurity

A dictionary that contains the device’s reduced security settings.

