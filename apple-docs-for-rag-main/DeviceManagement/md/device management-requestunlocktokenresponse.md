

- Device Management
-  RequestUnlockTokenResponse 

Device Management Command

# RequestUnlockTokenResponse

A response from the device after it processes a request for an unlock token.

iOS 5.0–6.1.6DeprecatediPadOS 5.0–6.1.6DeprecatedDevice Assignment ServicesVPP License Management

``` source
object RequestUnlockTokenResponse
```

## Properties

`CommandUUID`

`string`

Deprecated 

The unique identifier of the command for this response.

`EnrollmentID`

`string`

Deprecated   (Required) 

A per-enrollment device identifier for user enrollment.

`EnrollmentUserID`

`string`

Deprecated   (Required) 

A per-enrollment user identifier for user enrollment.

`ErrorChain`

`[`RequestUnlockTokenResponse.ErrorChainItem`]`

Deprecated 

An array of dictionaries that describes any errors that occurred.

`NotOnConsole`

`boolean`

Deprecated   (Required) 

If `true`, the device isn’t on-console.

`Status`

`string`

Deprecated   (Required) 

The status of the response, which is one of the following values:

- `Acknowledged`: The device processed the command successfully.

- `Error`: An error occurred. See the `ErrorChain` for more details.

- `CommandFormatError`: A protocol error occurred, which can result from a malformed command.

- `Idle`: The device is idle; there’s no status.

- `NotNow`: The device received the command, but couldn’t execute it.

Possible Values: `Acknowledged, Error, CommandFormatError, Idle, NotNow`

`UDID`

`string`

Deprecated   (Required) 

The unique identifier of the device.

`UnlockToken`

`data`

Deprecated   (Required) 

The unlock token. Erasing the user partition invalidates this token.

`UserID`

`string`

Deprecated 

For Shared iPad, this value is `FFFFFFFF-FFFF-FFFF-FFFF-FFFFFFFFFFFF` to indicate that authentication didn’t occur. In macOS, this value is the user identifier.

`UserLongName`

`string`

Deprecated   (Required) 

The full name of the user.

`UserShortName`

`string`

Deprecated 

For Shared iPad, this value is the Managed Apple ID of the user, which indicates the token is for the user channel. In macOS, this value is the short name of the user.

## Topics

### Commands

object RequestUnlockTokenResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object RequestUnlockTokenCommand

The command to request an unlock token from a device.

