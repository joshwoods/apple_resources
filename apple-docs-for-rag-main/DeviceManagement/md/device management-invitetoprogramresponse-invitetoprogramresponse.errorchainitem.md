

- Device Management
- InviteToProgramResponse
-  InviteToProgramResponse.ErrorChainItem 

Device Management Command

# InviteToProgramResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 7.0+iPadOS 7.0+macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object InviteToProgramResponse.ErrorChainItem
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

