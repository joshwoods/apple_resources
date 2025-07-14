

- Device Management
- UserListResponse
-  UserListResponse.UsersItem 

Device Management Command

# UserListResponse.UsersItem

A dictionary that contains information about an active account on a device.

iOS 9.3+iPadOS 9.3+macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object UserListResponse.UsersItem
```

## Properties

`DataQuota`

`integer`

 (Required) 

If present, the user’s data quota in bytes. This isn’t present if the account doesn’t enforce a quota. This value is available in iOS 9.3 and later.

`DataUsed`

`integer`

 (Required) 

The amount of data, in bytes, that the user has used. This value is available in iOS 9.3 and later.

`FullName`

`string`

 (Required) 

The user’s full name. This value is available in macOS 10.13 and later.

`HasDataToSync`

`boolean`

 (Required) 

If `true`, the user has data to sync to the cloud. This value is available in iOS 9.3 and later.

`HasSecureToken`

`boolean`

 (Required) 

If `true`, the user currently has a secure token set. This value is available in macOS 11 and later.

`IsLoggedIn`

`boolean`

 (Required) 

If `true`, the user is currently logged in on the device. This value is available in iOS 9.3 and later, and macOS 10.13 and later.

`MobileAccount`

`boolean`

 (Required) 

If `true`, the account is a mobile account. This value is available in macOS 10.13 and later.

`UID`

`integer`

 (Required) 

The user’s unique identifier. This value is available in macOS 10.13 and later.

`UserGUID`

`string`

 (Required) 

The user’s `GeneratedUID`. This value is available in macOS 10.13 and later.

`UserName`

`string`

 (Required) 

The user name for the account. In macOS, this is the short name of the user account. This value is available in iOS 9.3 and later, and macOS 10.13 and later.

## See Also

### Commands

object UserListResponse.ErrorChainItem

A dictionary that describes an error chain item.

