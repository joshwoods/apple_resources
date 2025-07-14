

- Device Management
- ErrorCodeSoftwareUpdateRequired
- ErrorCodeSoftwareUpdateRequired.Details
-  ErrorCodeSoftwareUpdateRequired.Details.RequireBetaProgram 

Object

# ErrorCodeSoftwareUpdateRequired.Details.RequireBetaProgram

A dictionary containing details of the beta program.

iOS 17.0+iPadOS 17.0+macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object ErrorCodeSoftwareUpdateRequired.Details.RequireBetaProgram
```

## Properties

`Description`

`string`

 (Required) 

A human readable description of the beta program.

`Token`

`string`

 (Required) 

The AxM seeding service token for the AxM organization the MDM server is part of. The system uses this token to enroll the device in the corresponding beta program.

