

- Device Management
- ManagedApplicationFeedbackResponse
-  ManagedApplicationFeedbackResponse.ErrorChainItem 

Device Management Command

# ManagedApplicationFeedbackResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 7.0+iPadOS 7.0+macOS 11.0+tvOS 10.2+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationFeedbackResponse.ErrorChainItem
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

## See Also

### Commands

object ManagedApplicationFeedbackResponse.ManagedApplicationFeedbackItem

A dictionary that contains a managed app’s feedback item.

