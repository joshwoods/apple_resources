

- Device Management
-  UserAuthenticateRequest 

Device Management Command

# UserAuthenticateRequest

The User Authenticate Request details.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object UserAuthenticateRequest
```

## Properties

`DigestResponse`

`string`

 (Required) 

A string provided by the client on second UserAuthenticate request after receiving `DigestChallenge` from server on first UserAuthenticate request.

`MessageType`

`string`

 (Required) 

The message type, which must have a value of `UserAuthenticate`.

Value: `UserAuthenticate`

`UDID`

`string`

 (Required) 

The device’s UDID (Unique Device ID).

`UserID`

`string`

 (Required) 

Local mobile user’s GUID or network user’s GUID from an Open Directory record.

