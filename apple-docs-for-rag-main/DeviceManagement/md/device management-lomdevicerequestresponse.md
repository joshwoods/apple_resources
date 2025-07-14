

- Device Management
-  LOMDeviceRequestResponse 

Device Management Command

# LOMDeviceRequestResponse

A response from the device after it processes requests it receives through lights-out management (LOM).

macOS 11.0+Device Assignment ServicesVPP License Management

``` source
object LOMDeviceRequestResponse
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

`[`LOMDeviceRequestResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

`NotOnConsole`

`boolean`

 (Required) 

If `true`, the device isn’t on-console.

`ResponseList`

`[`LOMDeviceRequestResponse.ResponseListItem`]`

 (Required) 

An array of dictionaries that describes the status of each request.

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

object LOMDeviceRequestResponse.ErrorChainItem

A dictionary that describes an error chain item.

object LOMDeviceRequestResponse.ResponseListItem

A dictionary that describes a response list item.

## See Also

### Command and Response

object LOMDeviceRequestCommand

The command to send requests to a device using lights-out management (LOM).

