

- Device Management
-  Create Users 

Web Service Endpoint

# Create Users

Create users to assign apps and books to.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/v2/users/create
```

## HTTP Body

ManageUsersRequest

missing

Content-Type: application/json

## Response Codes

` 200 ``OK`

EventResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

The provided token is invalid. It may either be missing or expired.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorResponse

`Internal Server Error`

An internal server error occurred. Try again later.

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
{
    "users": [
        {
            "clientUserId": "client-100",
            "email": "client-100@next.com",
            "managedAppleId": "maid-100@next.com"
        },
        {
            "clientUserId": "client-101",
            "email": "client-101@next.com",
            "managedAppleId": "maid-101@next.com"
        },
        {
            "clientUserId": "client-102",
            "email": "client-102@next.com"
        }
    ]
}
```

```
{
    "eventId": "af70eb9b-0ab6-405d-87d8-3b9ed0c4f370",
    "tokenExpirationDate": "2030-11-08T22:33:22+0000",
    "uId": "2049025000431439"
}
```

## Topics

### Request and Response

object ManageUsersRequest

The request for user management.

object EventResponse

The response that contains the event identifier.

object ErrorResponse

The response that contains the error that occurs.

## See Also

### User Management

Get Users

Get information about a set of users.

Update Users

Update details for existing users.

Retire Users

Retire users by client user IDs.

