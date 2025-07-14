

- Device Management
-  EditVppUserRequest 

Object

# EditVppUserRequest

The request to edit a user.

Device Assignment ServicesVPP License Management

``` source
object EditVppUserRequest
```

## Properties

`clientUserIdStr`

`string`

The identifier supplied by the client when registering a user. Either `clientUserIdStr` or `userId` is required. If both `clientUserIdStr` and `userId` are supplied, `userId` takes precedence.

`email`

`string`

The user’s email address. The `email` field is updated only if the value is provided in the request.

`itsIdHash`

`string`

The hash of the user’s iTunes Store ID.

`managedAppleIDStr`

`string`

The Apple ID associated with the user. This ID’s organization must match that of the provided sToken.

See Associating an Apple ID with a Volume Purchase Program (VPP) User for more information.

`sToken`

`string`

 (Required) 

The authentication token. For more information, see Authentication.

`userId`

`int64`

The unique identifier assigned by the VPP when registering the user. Either `clientUserIdStr` or `userId` is required. If both `clientUserIdStr` and `userId` are supplied, `userId` takes precedence.

## See Also

### Request and Response

object EditVppUserResponse

The response from editing a user.

