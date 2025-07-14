

- Device Management
-  Delete a User 

Web Service Endpoint

# Delete a User

Delete a user’s account from a device.

iOS 9.3+iPadOS 9.3+macOS 10.13+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#DeleteUserCommand
```

## HTTP Body

DeleteUserCommand

The command to delete a user’s account from a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

DeleteUserResponse

`OK`

A response from the device after it processes the command to delete a user’s account.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                    |
|----------------------------|--------------------|
| Device Channel             | macOS, Shared iPad |
| User Channel               | \-                 |
| Requires Supervision       | macOS              |
| Allowed in User Enrollment | \-                 |
| Required Access Right      | \-                 |

### Example Request and Response

- Request
- Response

```

    Command

        ForceDeletion

        RequestType
        DeleteUser
        UserName
        example@acme.com

    CommandUUID
    0001_DeleteUser

```

```

    CommandUUID
    0001_DeleteUser
    Status
    Acknowledged
    UDID
    cf98820bd143abe0bbf151bed8e8e427594d2f88

```

## Topics

### Command and Response

object DeleteUserCommand

The command to delete a user’s account from a device.

object DeleteUserResponse

A response from the device after it processes the command to delete a user’s account.

## See Also

### User Management

List the User Accounts

Get a list of users with active accounts on a device.

Log Out the User

Force the current user to log out of a device.

