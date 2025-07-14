

- Device Management
-  DeleteUserResponse 

Device Management Command

# DeleteUserResponse

A response from the device after it processes the command to delete a user’s account.

iOS 9.3+iPadOS 9.3+macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object DeleteUserResponse
```

## Properties

`CommandUUID`

`string`

The unique identifier of the command for this response.

`EnrollmentID`

`string`

 (Required) 

A per-enrollment device identifier for user enrollment.

`EnrollmentUserID`

`string`

 (Required) 

A per-enrollment user identifier for user enrollment.

`ErrorChain`

`[`DeleteUserResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

`NotOnConsole`

`boolean`

 (Required) 

If `true`, the device isn’t on-console.

`Status`

`string`

 (Required) 

The status of the response, which is either `Acknowledged`, or `Error` with one of the following error codes:

- `12071`: The user doesn’t exist.

- `12072`: The user is currently logged in.

- `12073`: The user has data to sync and `ForceDeletion` is `false` or unspecified.

- `12074`: Unable to delete the user. In macOS, this error code also returns for an attempt to delete the last administrator account.

Possible Values: `Acknowledged, Error, CommandFormatError, Idle, NotNow`

`UDID`

`string`

 (Required) 

The unique identifier of the device.

`UserID`

`string`

For Shared iPad, this value is `FFFFFFFF-FFFF-FFFF-FFFF-FFFFFFFFFFFF` to indicate that authentication didn’t occur. In macOS, this value is the user identifier.

`UserLongName`

`string`

 (Required) 

The full name of the user.

`UserShortName`

`string`

For Shared iPad, this value is the Managed Apple ID of the user, which indicates the token is for the user channel. In macOS, this value is the short name of the user.

## Topics

### Commands

object DeleteUserResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object DeleteUserCommand

The command to delete a user’s account from a device.

