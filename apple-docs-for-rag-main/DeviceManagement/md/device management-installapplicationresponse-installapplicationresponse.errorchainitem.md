

- Device Management
- InstallApplicationResponse
-  InstallApplicationResponse.ErrorChainItem 

Device Management Command

# InstallApplicationResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object InstallApplicationResponse.ErrorChainItem
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

