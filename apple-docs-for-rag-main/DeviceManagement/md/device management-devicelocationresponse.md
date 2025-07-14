

- Device Management
-  DeviceLocationResponse 

Device Management Command

# DeviceLocationResponse

A response from a device in Lost Mode after it processes the command to request its location.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

``` source
object DeviceLocationResponse
```

## Properties

`Altitude`

`number`

 (Required) 

The altitude of the device’s location, which is a negative value if the altitude is unknown.

`CommandUUID`

`string`

The unique identifier of the command for this response.

`Course`

`number`

 (Required) 

The direction the device is traveling, which is a negative value if the course is unknown.

`EnrollmentID`

`string`

 (Required) 

A per-enrollment device identifier for user enrollment.

`EnrollmentUserID`

`string`

 (Required) 

A per-enrollment user identifier for user enrollment.

`ErrorChain`

`[`DeviceLocationResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

`HorizontalAccuracy`

`number`

 (Required) 

The radius of uncertainty for the location in meters, which is a negative value if the horizontal accuracy is unknown.

`Latitude`

`number`

 (Required) 

The latitude of the device’s location.

`Longitude`

`number`

 (Required) 

The longitude of the device’s location.

`NotOnConsole`

`boolean`

 (Required) 

If `true`, the device isn’t on-console.

`Speed`

`number`

 (Required) 

The speed of the device in meters per second, which is a negative value if the speed is unknown.

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

`Timestamp`

`string`

 (Required) 

The RFC 3339 timestamp of when the server determined the location of the device.

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

`VerticalAccuracy`

`number`

 (Required) 

The accuracy of the altitude value in meters, which is a negative value if the vertical accuracy is unknown.

## Topics

### Commands

object DeviceLocationResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object DeviceLocationCommand

The command to request a device’s location.

