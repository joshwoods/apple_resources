

- Device Management
-  InstalledApplicationListResponse 

Device Management Command

# InstalledApplicationListResponse

A response from the device after it processes the command to get a list of installed apps.

iOS 5.0+iPadOS 5.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object InstalledApplicationListResponse
```

## Properties

`CommandUUID`

`string`

The unique identifier of the command.

`EnrollmentID`

`string`

 (Required) 

A per-enrollment device identifier for user enrollment.

`EnrollmentUserID`

`string`

 (Required) 

A per-enrollment user identifier for user enrollment.

`ErrorChain`

`[`InstalledApplicationListResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

`InstalledApplicationList`

`[`InstalledApplicationListResponse.InstalledApplicationListItem`]`

 (Required) 

An array of dictionaries that describes each installed app.

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

object InstalledApplicationListResponse.InstalledApplicationListItem

A dictionary that describes an app list item.

object InstalledApplicationListResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object InstalledApplicationListCommand

The command to get a list of installed apps on a device.

