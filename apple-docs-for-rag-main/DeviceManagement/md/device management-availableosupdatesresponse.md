

- Device Management
-  AvailableOSUpdatesResponse 

Device Management Command

# AvailableOSUpdatesResponse

A response from the device after it processes the command to get a list of available operating-system updates.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 12.0+Device Assignment ServicesVPP License Management

``` source
object AvailableOSUpdatesResponse
```

## Properties

`AvailableOSUpdates`

`[`AvailableOSUpdatesResponse.AvailableOSUpdatesItem`]`

 (Required) 

An array of dictionaries that contains only the most recent available updates in iOS and tvOS, and possibly multiple available updates in macOS. Follow the instructions in the Managed Apps and Updates section of the Apple Software Lookup Service to find a complete catalog of iOS and tvOS updates.

In macOS 14 and later, `AvailableOSUpdates` doesn’t include InstallAssistant-based, full-replacement installers. It only contains over-the-air (OTA) updates. OTA updates can update or upgrade the OS and support all `InstallAction` options.

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

`[`AvailableOSUpdatesResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

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

object AvailableOSUpdatesResponse.AvailableOSUpdatesItem

The response dictionary that describes the available operating-system updates item.

object AvailableOSUpdatesResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object AvailableOSUpdatesCommand

The command to get a list of available operating-system updates.

