

- Device Management
-  Get Users Deprecated

Web Service Endpoint

# Get Users

Get information about a set of users.

Device Assignment ServicesVPP License Management

Deprecated

This legacy API is currently in maintenance mode. Apple won’t add any new functionality to it.

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/getVPPUsersSrv
```

## HTTP Body

GetVppUsersRequest

missing

Content-Type: application/json

## Response Codes

` 200 ``OK`

GetVppUsersResponse

`OK`

Content-Type: application/json

## Mentioned in 

Retrieving a Large Record Set

Handling Error Responses

## Discussion

### Example Request and Response

- Request
- Response

```
{
  "batchToken": null,
  "sinceModifiedToken": null,
  "includeRetired": 1,
  "includeRetiredOnly": false,
  "ifModifiedSince": null,
  "overrideIndex": null,
  "sToken": "h40Gte9aQnZFDNM39IUkRPCsQDxBxbZB4Wy34pxefOuQkeeb3h2 a5Rlopo4KDn3MrFKf4CM3OY+WGAoZ1cD6iZ6yzsMk1+5PVBNc66YS6ZQ="
}
```

```
{
  "clientContext": "{\"guid\":\"b92\",\"hostname\":\"test.test.org\",\"ac2\":1}",
  "batchCount": 4,
  "expirationMillis": 1898103480266,
  "location": {
    "locationId": 22222222222,
    "locationName": "LocationName"
  },
  "sinceModifiedToken": "H4sIAAAAAAAAAKtWMFCwVdBQMDQwMDEwV9C0VlAoyS9JzHFKLEnOSC12yy/NS3EGEiVAVYZAycw03/yUzLTM1JTgzLzkVN/MnJzMYpCcqamJiaGlkbGBiakZiiEw3QYg0cqCVCBTqRisF2qQEsjYvOSc0pTUoNSSzKLUFIhdtQAHYCyLnAAAAA==",
  "status": 0,
  "totalBatchCount": "0",
  "totalCount": 4,
  "uId": "100978",
  "users": [
    {
      "userId": 1,
      "email": "user1@test.com",
      "clientUserIdStr": "200006",
      "status": "Associated",
      "itsIdHash": "C2Wwd8LcIaE2v6f2/mvu82Gs/Lc="
    },
    {
      "userId": 2,
      "email": "user2@test.com",
      "clientUserIdStr": "200007",
      "status": "Associated",
      "itsIdHash": "*leSKk3IaE2vk2KLmv2k3/200D3="
    },
    {
      "userId": 3,
      "email": "user3@test.com",
      "clientUserIdStr": "user3@test.com",
      "status": "Registered",
      "inviteCode": "f551b37da07146628e8dcbe0111f0364",
      "inviteUrl": "https://buy.itunes.apple.com/WebObjects/MZFinance.woa/wa/associateVPPUserWithITSAccount?inviteCode=f551b37da07146628e8dcbe0111f0364&mt=8"
    },
    {
      "userId": 4,
      "email": "user4@test.com",
      "clientUserIdStr": "user4@test.com",
      "status": "Registered",
      "inviteUrl": "https://buy.itunes.apple.com/WebObjects/MZFinance.woa/wa/associateVPPUserWithITSAccount?inviteCode=859c5aa3485a48918a5f4f70c5629ec8&mt=8",
      "inviteCode": "859c5aa3485a48918a5f4f70c5629ec8"
    }
  ]
}
```

## Topics

### Request and Response

object GetVppUsersRequest

The request for the users’ details service.

object GetVppUsersResponse

The response from the users’ details service.

## See Also

### User Management

Get a User

Get information about a particular user.

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

