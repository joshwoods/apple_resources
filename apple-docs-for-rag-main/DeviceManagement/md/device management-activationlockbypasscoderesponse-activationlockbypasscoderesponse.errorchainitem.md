

- Device Management
- ActivationLockBypassCodeResponse
-  ActivationLockBypassCodeResponse.ErrorChainItem 

Device Management Command

# ActivationLockBypassCodeResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 7.1+iPadOS 7.1+macOS 10.15+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object ActivationLockBypassCodeResponse.ErrorChainItem
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

