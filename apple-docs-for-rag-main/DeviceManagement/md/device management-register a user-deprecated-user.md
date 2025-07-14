

- Device Management
-  Register a User Deprecated

Web Service Endpoint

# Register a User

Register a user with the volume-purchase program.

Device Assignment ServicesVPP License Management

Deprecated

This legacy API is currently in maintenance mode. Apple won’t add any new functionality to it.

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/registerVPPUserSrv
```

## HTTP Body

RegisterVppUserRequest

missing

Content-Type: application/json

## Response Codes

` 200 ``OK`

RegisterVppUserResponse

`OK`

Content-Type: application/json

## Mentioned in 

Associating an Apple ID with a Volume Purchase Program (VPP) User

## Discussion

### Example Request and Response

- Request
- Response

```
{
  "email": "test_reg_user11@test.com",
  "clientUserIdStr": "200002",
  "sToken": "h40Gte9aQnZFDNM39IUkRPCsQDxBxbZB4Wy34pxefOuQkeeb3h2a5Ropo4KDn3MKf4CM3OY+WGAoZ1cD6iZ6yzsMk1+5PVBNc66YS6ZQ="
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
    "clientUserIdStr": "200002",
    "email": "test_reg_user11@test.com",
    "inviteCode": "9e8d1ecc57924d9da13b42b4f772a066",
    "inviteUrl": "https://buy.itunes.apple.com/WebObjects/MZFinance.woa/wa/associateVPPUserWithITSAccount?cc=us&inviteCode= 89e8d1ecc57924d9da13b42b4f772a066&mt=8",
    "status": "Registered",
    "userId": 100014
  }
}
```

## Topics

### Request and Response

object RegisterVppUserRequest

The request for registering a user.

object RegisterVppUserResponse

The response from registering a user.

## See Also

### User Management

Get a User

Get information about a particular user.

Deprecated

Get Users

Get information about a set of users.

Deprecated

Edit a User

Modify details about a user.

Deprecated

Retire a User

Retire a user account.

Deprecated

