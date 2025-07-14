

- Device Management
-  LOMSetupRequestResponse 

Device Management Command

# LOMSetupRequestResponse

A response from the device after it processes the command to get setup information for lights-out management (LOM).

macOS 11.0+Device Assignment ServicesVPP License Management

``` source
object LOMSetupRequestResponse
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

`[`LOMSetupRequestResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

`LOMProtocolVersion`

`integer`

 (Required) 

The LOM protocol version that the device supports.

`NotOnConsole`

`boolean`

 (Required) 

If `true`, the device isn’t on-console.

`PrimaryIPv6AddressList`

`[string]`

 (Required) 

An array that contains the IPv6 addresses for primary LOM-compatible Ethernet interfaces for the device.

`SecondaryIPv6AddressList`

`[string]`

 (Required) 

An array that contains the IPv6 addresses for secondary LOM-compatible Ethernet interfaces for the device.

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

object LOMSetupRequestResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object LOMSetupRequestCommand

The command to get information from a device to set up lights-out management (LOM).

