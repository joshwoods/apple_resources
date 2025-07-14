

- Device Management
- ClearActivationLockBypassCodeResponse
-  ClearActivationLockBypassCodeResponse.ErrorChainItem 

Device Management Command

# ClearActivationLockBypassCodeResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 7.1+iPadOS 7.1+macOS 10.15+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object ClearActivationLockBypassCodeResponse.ErrorChainItem
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

