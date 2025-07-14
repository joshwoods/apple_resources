

- Device Management
-  Retire a User Deprecated

Web Service Endpoint

# Retire a User

Retire a user account.

Device Assignment ServicesVPP License Management

Deprecated

This legacy API is currently in maintenance mode. Apple won’t add any new functionality to it.

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/retireVPPUserSrv
```

## HTTP Body

RetireVppUserRequest

missing

Content-Type: application/json

## Response Codes

` 200 ``OK`

RetireVppUserResponse

`OK`

Content-Type: application/json

## Discussion

This service disassociates a VPP user from its iTunes account and releases the revocable licenses associated with the VPP user. The revoked licenses can then be assigned to other users in the organization.

Currently, ebook licenses are irrevocable.

A retired VPP user can be reregistered, in the same organization, using the Register a User endpoint.

### Example Request and Response

- Request
- Response

```
{
  "userId": 1,
  "sToken": "h40Gte9aQnZFDNM39IUkRPCsQDxBxbZB4Wy34pxefOuQkeeb3h2a5Rlopo4KDn3MrFKf4CM3OY+WGAoZ1cD6iZ6yzsMk1+5PVBNc66YS6ZQ="
}
```

```
{
  "clientContext": "{\"guid\":\"b92\",\"hostname\":\"test.test.org\",\"ac2\":1}",
  "expirationMillis": 1898103480266,
  "location": {
    "locationId": 22222222222,
    "locationName": "LocationName"
  },
  "status": 0,
  "uId": "100978",
  "user": {
    "clientUserIdStr": "200006",
    "email": "user1@test.com",
    "licenses": [
      {
        "licenseId": 2,
        "adamId": 408709785,
        "productTypeId": 10,
        "pricingParam": "STDQ",
        "productTypeName": "Publication",
        "isIrrevocable": true
      }
    ],
    "status": "Retired",
    "userId": 1
  }
}
```

## Topics

### Request and Response

object RetireVppUserRequest

The request to retire a user.

object RetireVppUserResponse

The response from retiring a user.

## See Also

### User Management

Get a User

Get information about a particular user.

Deprecated

Get Users

Get information about a set of users.

Deprecated

Register a User

Register a user with the volume-purchase program.

Deprecated

Edit a User

Modify details about a user.

Deprecated

