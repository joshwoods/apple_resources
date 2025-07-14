

- Device Management
- PlayLostModeSoundResponse
-  PlayLostModeSoundResponse.ErrorChainItem 

Device Management Command

# PlayLostModeSoundResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 10.3+iPadOS 10.3+Device Assignment ServicesVPP License Management

``` source
object PlayLostModeSoundResponse.ErrorChainItem
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

