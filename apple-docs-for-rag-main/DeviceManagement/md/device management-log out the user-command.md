

- Device Management
-  Log Out the User 

Web Service Endpoint

# Log Out the User

Force the current user to log out of a device.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#LogOutUserCommand
```

## HTTP Body

LogOutUserCommand

The command to force the current user to log out of a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

LogOutUserResponse

`OK`

A response from the device after it processes the command to force the current user to log out.

Content-Type: application/xml

## Discussion

After logging out the user, MDM commands aren’t available on the device for up to 2 minutes.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |             |
|----------------------------|-------------|
| Device Channel             | Shared iPad |
| User Channel               | \-          |
| Requires Supervision       | \-          |
| Allowed in User Enrollment | \-          |
| Required Access Right      | \-          |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        LogOutUser

    CommandUUID
    0001_LogOutUser

```

```

    CommandUUID
    0001_LogOutUser
    Status
    Acknowledged
    UDID
    cf98820bd143abe0bbf151bed8e8e427594d2f88

```

## Topics

### Command and Response

object LogOutUserCommand

The command to force the current user to log out of a device.

object LogOutUserResponse

A response from the device after it processes the command to force the current user to log out.

## See Also

### User Management

List the User Accounts

Get a list of users with active accounts on a device.

Delete a User

Delete a user’s account from a device.

