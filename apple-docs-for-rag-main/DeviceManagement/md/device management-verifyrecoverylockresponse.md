

- Device Management
-  VerifyRecoveryLockResponse 

Device Management Command

# VerifyRecoveryLockResponse

A response from the device after it verifies the password for Recovery Lock.

macOS 11.5+Device Assignment ServicesVPP License Management

``` source
object VerifyRecoveryLockResponse
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

`[`VerifyRecoveryLockResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occur.

`NotOnConsole`

`boolean`

 (Required) 

If `true`, the device isn’t on-console.

`PasswordVerified`

`boolean`

 (Required) 

If `true`, the device verified the password.

`Status`

`string`

 (Required) 

The status of the response, which is one of the following values:

- `Acknowledged`: The device processed the command successfully.

- `Error`: An error occurred. See the `ErrorChain` for more details.

- `CommandFormatError`: A protocol error occurred, which can result from a malformed command.

- `Idle`: The device is idle, so there’s no status.

- `NotNow`: The device received the command, but couldn’t execute it.

Possible Values: `Acknowledged, Error, CommandFormatError, Idle, NotNow`

`UDID`

`string`

 (Required) 

The unique identifier of the device.

`UserID`

`string`

For Shared iPad, this value is `FFFFFFFF-FFFF-FFFF-FFFF-FFFFFFFFFFFF` to indicate when verification doesn’t occur. In macOS, this value is the user identifier.

`UserLongName`

`string`

 (Required) 

The full name of the user.

`UserShortName`

`string`

For Shared iPad, this value is the Managed Apple ID of the user, which indicates the token is for the user channel. In macOS, this value is the short name of the user.

## Topics

### Commands

object VerifyRecoveryLockResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object VerifyRecoveryLockCommand

The command to verify the password for Recovery Lock.

