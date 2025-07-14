

- Device Management
- ProvisioningProfileListResponse
-  ProvisioningProfileListResponse.ErrorChainItem 

Device Management Command

# ProvisioningProfileListResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 4.0+iPadOS 4.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ProvisioningProfileListResponse.ErrorChainItem
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

object ProvisioningProfileListResponse.ProvisioningProfileListItem

A dictionary that describes a provisioning profile list item.

