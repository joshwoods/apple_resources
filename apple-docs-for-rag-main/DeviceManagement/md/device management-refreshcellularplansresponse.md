

- Device Management
-  RefreshCellularPlansResponse 

Device Management Command

# RefreshCellularPlansResponse

A response from the device after it processes the command to query a carrier URL for active eSIM cellular-plan profiles.

iOS 13.0+iPadOS 13.0+Device Assignment ServicesVPP License Management

``` source
object RefreshCellularPlansResponse
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

`[`RefreshCellularPlansResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

`NotOnConsole`

`boolean`

 (Required) 

If `true`, the device isn’t on-console.

`Status`

`string`

 (Required) 

The status of the response, which is either `Acknowledged`, or `Error` with one of the following errors:

- `36001`: Unable to communicate with the cellular software stack.

- `36002`: The hardware doesn’t support this command.

- `36003`: The cellular stack was unable to perform the request. This error can also occur if the cellular stack is busy, in which case, retrying the command later may resolve the issue.

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

object RefreshCellularPlansResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object RefreshCellularPlansCommand

The command to query a carrier URL for active eSIM cellular-plan profiles.

