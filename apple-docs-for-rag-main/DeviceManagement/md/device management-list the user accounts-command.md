

- Device Management
-  List the User Accounts 

Web Service Endpoint

# List the User Accounts

Get a list of users with active accounts on a device.

iOS 9.3+iPadOS 9.3+macOS 10.13+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#UserListCommand
```

## HTTP Body

UserListCommand

The command to get a list of users with active accounts on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

UserListResponse

`OK`

A response from the device after it processes the command to get a list of users with active accounts.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Query Availability

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

        RequestType
        UserList

    CommandUUID
    0001_UserList

```

```

    CommandUUID
    0001_UserList
    Status
    Acknowledged
    UDID
    cf98820bd143abe0bbf151bed8e8e427594d2f88
    Users

            DataQuota
            10171187200
            DataUsed
            145625088
            HasDataToSync

            IsLoggedIn

            UserName
            example@acme.com

```

## Topics

### Command and Response

object UserListCommand

The command to get a list of users with active accounts on a device.

object UserListResponse

A response from the device after it processes the command to get a list of users with active accounts.

## See Also

### User Management

Log Out the User

Force the current user to log out of a device.

Delete a User

Delete a user’s account from a device.

