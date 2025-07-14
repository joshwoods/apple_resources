

- Device Management
- ValidateApplicationsResponse
-  ValidateApplicationsResponse.ErrorChainItem 

Device Management Command

# ValidateApplicationsResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 9.2+iPadOS 9.2+tvOS 10.2+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object ValidateApplicationsResponse.ErrorChainItem
```

## Properties

`ErrorCode`

`integer`

 (Required) 

The error code.

`ErrorDomain`

`string`

 (Required) 

The error domain.

`LocalizedDescription`

`string`

 (Required) 

A description of the error in the device’s localized language.

`USEnglishDescription`

`string`

A description of the error in U.S. English.

