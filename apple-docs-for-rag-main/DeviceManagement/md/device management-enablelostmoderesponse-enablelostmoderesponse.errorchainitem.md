

- Device Management
- EnableLostModeResponse
-  EnableLostModeResponse.ErrorChainItem 

Device Management Command

# EnableLostModeResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

``` source
object EnableLostModeResponse.ErrorChainItem
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

