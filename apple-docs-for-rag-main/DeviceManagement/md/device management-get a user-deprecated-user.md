

- Device Management
-  Get a User Deprecated

Web Service Endpoint

# Get a User

Get information about a particular user.

Device Assignment ServicesVPP License Management

Deprecated

This legacy API is currently in maintenance mode. Apple won’t add any new functionality to it.

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/getVPPUserSrv
```

## HTTP Body

GetVppUserRequest

missing

Content-Type: application/json

## Response Codes

` 200 ``OK`

GetVppUserResponse

`OK`

Content-Type: application/json

## Discussion

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
    "inviteCode": "201d8c3d520e4b34bec3ed49f20b5b8a",
    "inviteUrl": "https://buy.itunes.apple.com/WebObjects/MZFinance.woa/wa/associateVPPUserWithITSAccount?cc=us&inviteCode=201d8c3d520e4b34bec3ed49f20b5b8a&mt=8",
    "itsIdHash": "C2Wwd8LcIaE2v6f2/mvu82Gs/Lc=",
    "licenses":[
         {
            "licenseId":2,
            "adamId":408709785,
            "productTypeId":7,
            "pricingParam":"STDQ",
            "productTypeName":"Software",
            "isIrrevocable":false
         },
         {
            "licenseId":4,
            "adamId":497799835,
            "productTypeId":7,
            "pricingParam":"STDQ",
            "productTypeName":"Software",
            "isIrrevocable":false
         }
      ],
    "status": "Registered",
    "userId": 1
  }
}
```

## Topics

### Request and Response

object GetVppUserRequest

The request for the user details service.

object GetVppUserResponse

The response from the user details service.

## See Also

### User Management

Get Users

Get information about a set of users.

Deprecated

Register a User

Register a user with the volume-purchase program.

Deprecated

Edit a User

Modify details about a user.

Deprecated

Retire a User

Retire a user account.

Deprecated

