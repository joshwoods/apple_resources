

- Device Management
-  Edit a User Deprecated

Web Service Endpoint

# Edit a User

Modify details about a user.

Device Assignment ServicesVPP License Management

Deprecated

This legacy API is currently in maintenance mode. Apple won’t add any new functionality to it.

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/editVPPUserSrv
```

## HTTP Body

EditVppUserRequest

missing

Content-Type: application/json

## Response Codes

` 200 ``OK`

EditVppUserResponse

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
  "userId": 100014,
  "email": "test_reg_user15_edited@test.com",
  "sToken": "h40Gte9aQnZFDNM39IUkRPCsQDxBxbZB4Wy34pxefOuQkeeb3h2a5Rlopo4KDn3MFKf4CM3OY+WGAoZ1cD6iZ6yzsMk1+5PVBNc66YS6ZQ="
}
```

```
{
  "clientContext": "{\"guid\":\"b92\",\"hostname\":\"test.test.org\",\"ac2\":1}",
  "expirationMillis": 1898103480266,
  "location": {
    "locationId": 2000000003431864,
    "locationName": "cloudMDM Location"
  },
  "status": 0,
  "uId": "100978",
  "user": {
    "clientUserIdStr": "200015",
    "email": "test_reg_user15_edited@test.com",
    "inviteCode": "9e8d1ecc57924d9da13b42b4f772a066",
    "inviteUrl": "https://buy.itunes.apple.com/WebObjects/MZFinance.woa/wa/associateVPPUserWithITSAccount?cc=us&inviteCode=9e8d1ecc57924d9da13b42b4f772a066&mt=8",
    "itsIdHash": "C2Wwd8LcIaE2v6f2/mvu82Gs/Lc="
    "status": "Registered",
    "userId": 100014
  }
}
```

## Topics

### Request and Response

object EditVppUserRequest

The request to edit a user.

object EditVppUserResponse

The response from editing a user.

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

Retire a User

Retire a user account.

Deprecated

