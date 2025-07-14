

- Device Management
-  Retire Users 

Web Service Endpoint

# Retire Users

Retire users by client user IDs.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/v2/users/retire
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
            "clientUserId": "client-100"
        },
        {
            "clientUserId": "client-101"
        }
    ]
}
```

```
{
    "eventId": "dafdad60-4ef6-49b0-8150-64323f56d88d",
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

Create Users

Create users to assign apps and books to.

Update Users

Update details for existing users.

