

- Device Management
- ProfileListResponse
-  ProfileListResponse.ErrorChainItem 

Device Management Command

# ProfileListResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ProfileListResponse.ErrorChainItem
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

object ProfileListResponse.ProfileListItem

A dictionary that describes a profile list item.

object ProfileListResponse.ProfileListItem.PayloadContentItem

A dictionary that describes a profile payload content item.

