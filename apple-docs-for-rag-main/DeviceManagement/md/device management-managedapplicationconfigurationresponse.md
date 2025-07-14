

- Device Management
-  ManagedApplicationConfigurationResponse 

Device Management Command

# ManagedApplicationConfigurationResponse

A response from the device after it processes the command to get app configurations from managed apps.

iOS 7.0+iPadOS 7.0+macOS 10.15+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationConfigurationResponse
```

## Properties

`ApplicationConfigurations`

`[`ManagedApplicationConfigurationResponse.ApplicationConfigurationsItem`]`

 (Required) 

An array of app configurations items.

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

`[`ManagedApplicationConfigurationResponse.ErrorChainItem`]`

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

object ManagedApplicationConfigurationResponse.ApplicationConfigurationsItem

A dictionary that contains a managed app’s configurations item.

object ManagedApplicationConfigurationResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object ManagedApplicationConfigurationCommand

The command to get managed app configurations on a device.

