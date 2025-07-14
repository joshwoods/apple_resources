

- Device Management
-  GetTokenRequest 

Device Management Command

# GetTokenRequest

Check-in protocol get-token request data.

iOS 17.0+iPadOS 17.0+macOS 14.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object GetTokenRequest
```

## Properties

`EnrollmentID`

`string`

 (Required) 

A per-enrollment identifier that identifies the device for user enrollments.

`EnrollmentUserID`

`string`

 (Required) 

A per-enrollment identifier that identifies the user for user enrollments.

`MessageType`

`string`

 (Required) 

A string that specifies this is a get-token request.

Value: `GetToken`

`TokenParameters`

GetTokenRequest.TokenParameters

Parameters that the system uses to generate the token.

`TokenServiceType`

`string`

 (Required) 

A string that specifies the service for the requested token.

Possible Values: `com.apple.maid, com.apple.watch.pairing`

`UDID`

`string`

 (Required) 

The device’s UDID.

`UserID`

`string`

In macOS, this value returns the ID of the user. On Shared iPad, this value is `FFFFFFFF-FFFF-FFFF-FFFF-FFFFFFFFFFFF` to indicate that no authentication occurs.

`UserLongName`

`string`

 (Required) 

The full name of the user.

`UserShortName`

`string`

On Shared iPad, this value returns the Managed Apple ID of the user. When present, it indicates that the token is for the user channel. In macOS, this value returns the short name of the user.

## Topics

### Supporting Objects

object GetTokenRequest.TokenParameters

Parameters that the system uses to generate the token.

## See Also

### Request and Response

object GetTokenResponse

Check-in protocol get-token response data.

