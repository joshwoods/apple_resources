

- Device Management
- UserListResponse
-  UserListResponse.ErrorChainItem 

Device Management Command

# UserListResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 9.3+iPadOS 9.3+macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object UserListResponse.ErrorChainItem
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

object UserListResponse.UsersItem

A dictionary that contains information about an active account on a device.

