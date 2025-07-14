

- Device Management
- ErrorCodeSoftwareUpdateRequired
-  ErrorCodeSoftwareUpdateRequired.Details 

Object

# ErrorCodeSoftwareUpdateRequired.Details

A dictionary that contains additional data about the software update required error code.

iOS 17.0+iPadOS 17.0+macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object ErrorCodeSoftwareUpdateRequired.Details
```

## Properties

`BuildVersion`

`string`

The build version that the device needs to update to, for example, “20A242. The systems uses the build version for testing during seeding periods. This identifier can include a supplemental version identifier, for example, “20A242a”. If the `BuildVersion` isn’t consistent with the `OSVersion`, `OSVersion` take precedence.

`OSVersion`

`string`

 (Required) 

The OS version that the device needs to update to, for example, “16.1”. This identifier can include a supplemental version identifier, for example, “16.1 (a)”.

`RequireBetaProgram`

ErrorCodeSoftwareUpdateRequired.Details.RequireBetaProgram

The device enrolls in the beta program, allowing enforced software updates to beta program OS versions. The device remains in the beta program after the system completes the enforced software update.

## Topics

### Objects

object ErrorCodeSoftwareUpdateRequired.Details.RequireBetaProgram

A dictionary containing details of the beta program.

