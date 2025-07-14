

- Device Management
- SecurityInfoResponse
- SecurityInfoResponse.SecurityInfo
-  SecurityInfoResponse.SecurityInfo.ManagementStatus 

Device Management Command

# SecurityInfoResponse.SecurityInfo.ManagementStatus

A dictionary that contains the status of the device’s MDM enrollment.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SecurityInfoResponse.SecurityInfo.ManagementStatus
```

## Properties

`EnrolledViaDEP`

`boolean`

If `true`, the device enrolled in MDM through the Device Enrollment Program (DEP). This value is available in macOS 10.13.2 and later.

`IsActivationLockManageable`

`boolean`

If `true`, the type of enrollment allows the MDM to manage Activation Lock for this device. This value is available in macOS 10.15 and later.

`IsUserEnrollment`

`boolean`

If `true`, the device is user-enrolled. This value is available in iOS 13 and later, and macOS 10.15 and later.

`UserApprovedEnrollment`

`boolean`

If `true`, the enrollment was user-approved. If `false`, the device may reject certain security-sensitive payloads or commands. This value is available in macOS 10.13.2 and later.

## See Also

### Commands

object SecurityInfoResponse.SecurityInfo.FirewallSettings

A dictionary that contains the firewall settings.

object SecurityInfoResponse.SecurityInfo.FirmwarePasswordStatus

A dictionary that contains the status of the EFI firmware password.

object SecurityInfoResponse.SecurityInfo.SecureBoot

The response object for the secure boot settings.

object SecurityInfoResponse.SecurityInfo.SecureBoot.ReducedSecurity

A dictionary that contains the device’s reduced security settings.

