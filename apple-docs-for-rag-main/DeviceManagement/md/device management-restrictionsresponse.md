

- Device Management
-  RestrictionsResponse 

Device Management Command

# RestrictionsResponse

A response from the device after it processes the command to get a list of restrictions.

iOS 4.0+iPadOS 4.0+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object RestrictionsResponse
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

`[`RestrictionsResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

`GlobalRestrictions`

RestrictionsResponse.GlobalRestrictions

 (Required) 

A dictionary that contains the global restrictions in effect. This value is available in iOS 4 and later, and tvOS 6.1 and later.

`NotOnConsole`

`boolean`

 (Required) 

If `true`, the device isn’t on-console.

`ProfileRestrictions`

RestrictionsResponse.ProfileRestrictions

 (Required) 

A dictionary that contains dictionaries of restrictions from each profile. This value is only available when `ProfileRestrictions` is `true` in the command. The keys are the identifiers of the profiles. This value is available in iOS 4 and later, and tvOS 6.1 and later.

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

object RestrictionsResponse.GlobalRestrictions

A dictionary that contains the global restrictions in effect.

object RestrictionsResponse.ProfileRestrictions

A dictionary that contains restrictions from each profile.

object RestrictionsResponse.ErrorChainItem

A dictionary that describes an error chain.

## See Also

### Command and Response

object RestrictionsCommand

The command to get a list of restrictions on a device.

