

- Device Management
-  InviteToProgramResponse 

Device Management Command

# InviteToProgramResponse

A response from the device after it processes the command to invite a user to join the Volume Purchase Program (VPP).

iOS 7.0+iPadOS 7.0+macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object InviteToProgramResponse
```

## Properties

`CommandUUID`

`string`

The unique identifier of the command for this response.

`EnrollmentID`

`string`

 (Required) 

A per-enrollment device identifier for user enrollment.

`ErrorChain`

`[`InviteToProgramResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

`EnrollmentUserID`

`string`

 (Required) 

A per-enrollment user identifier for user enrollment.

`InvitationResult`

`string`

 (Required) 

The result of the command.

Possible Values: `Acknowledged, InvalidProgramID, InvalidInvitationURL`

`NotOnConsole`

`boolean`

 (Required) 

If `true`, the device isn’t on-console.

`Status`

`string`

 (Required) 

The status of the response, which is one of the following values:

- `Acknowledged`: The device processed the command successfully.

- `Error`: An error occurred. See the `ErrorChain` for more details.

- `CommandFormatError`: A protocol error occurred, which can result from a malformed command.

- `Idle`: The device is idle; there’s no status.

- `NotNow`: The device received the command, but couldn’t execute it.

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

object InviteToProgramResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object InviteToProgramCommand

The command to invite a user on a device to join the Volume Purchase Program (VPP).

