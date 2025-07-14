

- Device Management
- SecurityInfoResponse
- SecurityInfoResponse.SecurityInfo
- SecurityInfoResponse.SecurityInfo.SecureBoot
-  SecurityInfoResponse.SecurityInfo.SecureBoot.ReducedSecurity 

Device Management Command

# SecurityInfoResponse.SecurityInfo.SecureBoot.ReducedSecurity

A dictionary that contains the device’s reduced security settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SecurityInfoResponse.SecurityInfo.SecureBoot.ReducedSecurity
```

## Properties

`AllowsAnyAppleSignedOS`

`string`

If `true`, allows any signed version of trusted system software from Apple to run.

`AllowsMDM`

`string`

If `true`, the MDM server controls kernel extensions and software updates.

`AllowsUserKextApproval`

`string`

If `true`, the user has control over kernel extensions.

## See Also

### Commands

object SecurityInfoResponse.SecurityInfo.FirewallSettings

A dictionary that contains the firewall settings.

object SecurityInfoResponse.SecurityInfo.FirmwarePasswordStatus

A dictionary that contains the status of the EFI firmware password.

object SecurityInfoResponse.SecurityInfo.ManagementStatus

A dictionary that contains the status of the device’s MDM enrollment.

object SecurityInfoResponse.SecurityInfo.SecureBoot

The response object for the secure boot settings.

