

- Device Management
-  OSUpdateStatusResponse 

Device Management Command

# OSUpdateStatusResponse

A response from the device after it processes the command to get the status of operating-system updates.

iOS 9.0+iPadOS 9.0+macOS 10.11.5+tvOS 12.0+Device Assignment ServicesVPP License Management

``` source
object OSUpdateStatusResponse
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

`[`OSUpdateStatusResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

`NotOnConsole`

`boolean`

 (Required) 

If `true`, the device isn’t on-console.

`OSUpdateStatus`

`[`OSUpdateStatusResponse.OSUpdateStatusItem`]`

 (Required) 

An array of dictionaries that describes the statuses of software updates. The array is empty if there are no software updates currently in progress.

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

object OSUpdateStatusResponse.OSUpdateStatusItem

A dictionary that describes the status of a software update.

object OSUpdateStatusResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object OSUpdateStatusCommand

The command to get the status of operating-system updates.

