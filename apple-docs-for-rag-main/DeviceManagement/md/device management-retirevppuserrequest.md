

- Device Management
-  RetireVppUserRequest 

Object

# RetireVppUserRequest

The request to retire a user.

Device Assignment ServicesVPP License Management

``` source
object RetireVppUserRequest
```

## Properties

`clientUserIdStr`

`string`

The identifier supplied by the client when registering a user. Either `clientUserIdStr` or `userId` is required. If both `clientUserIdStr` and `userId` are supplied, `userId` takes precedence.

`sToken`

`string`

 (Required) 

The authentication token. For more information, see Authentication.

`userId`

`int64`

The unique identifier assigned by the VPP when registering the user. Either `clientUserIdStr` or `userId` is required. If both `clientUserIdStr` and `userId` are supplied, `userId` takes precedence.

## See Also

### Request and Response

object RetireVppUserResponse

The response from retiring a user.

