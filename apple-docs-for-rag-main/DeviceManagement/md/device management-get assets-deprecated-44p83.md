

- Device Management
-  Get Assets Deprecated

Web Service Endpoint

# Get Assets

Get the set of assets managed by your organization.

Device Assignment ServicesVPP License Management

Deprecated

This legacy API is currently in maintenance mode. Apple won’t add any new functionality to it.

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/getVPPAssetsSrv
```

## HTTP Body

GetVppAssetRequest

missing

Content-Type: application/json

## Response Codes

` 200 ``OK`

GetVppAssetResponse

`OK`

Content-Type: application/json

## Mentioned in 

Upgrading to Apple School Manager (ASM) and Apple Business Manager (ABM)

Handling Error Responses

## Discussion

### Example Request and Response

- Request
- Response

```
{
  "sToken": "h40Gte9aQnZFDNM39IUkRPCsQDxBxbZB4Wy34pxefOuQkeeb3h2 a5Rlopo4KDn3MrFKf4CM3OY+WGAoZ1cD6iZ6yzsMk1+5PVBNc66YS6ZQ=",
  "includeLicenseCounts": true,
  "pricingParam": null
}
```

```
{
  "assets": [
    {
      "adamIdStr": "748057890",
      "assignedCount": 0,
      "availableCount": 25,
      "deviceAssignable": true,
      "isIrrevocable": false,
      "pricingParam": "STDQ",
      "productTypeId": 8,
      "productTypeName": "Application",
      "retiredCount": 0,
      "totalCount": 25
    },
    {
      "adamIdStr": "635851129",
      "assignedCount": 0,
      "availableCount": 40,
      "deviceAssignable": true,
      "isIrrevocable": false,
      "pricingParam": "STDQ",
      "productTypeId": 8,
      "productTypeName": "Application",
      "retiredCount": 0,
      "totalCount": 40
    },
    {
      "adamIdStr": "284035177",
      "assignedCount": 0,
      "availableCount": 0,
      "deviceAssignable": false,
      "isIrrevocable": false,
      "pricingParam": "STDQ",
      "productTypeId": 8,
      "productTypeName": "Application",
      "retiredCount": 10,
      "totalCount": 0
    }
  ],
  "clientContext": "{\"guid\":\"b92\",\"hostname\":\"test.test.org\",\"ac2\":1}",
   "location": {
    "locationId": 22222222222,
    "locationName": "LocationName"
  },
  "expirationMillis": 1898103480266,
  "status": 0,
  "totalCount": 3,
  "uId": "103614"
}
```

### Example Request and Response with a Legacy Token

- Request
- Response

```
{
  "sToken": "h40Gte9aQnZFDNM39IUkRPCsQDxBxbZB4Wy34pxefOuQkeeb3h2 a5Rlopo4KDn3MrFKf4CM3OY+WGAoZ1cD6iZ6yzsMk1+5PVBNc66YS6ZQ=",
  "includeLicenseCounts": true,
  "pricingParam": null
}
```

```
{
  "assets": [
    {
      "adamIdStr": "748057890",
      "assignedCount": 0,
      "availableCount": 10,
      "deviceAssignable": true,
      "isIrrevocable": false,
      "pricingParam": "STDQ",
      "productTypeId": 8,
      "productTypeName": "Application",
      "retiredCount": 0,
      "totalCount": 10
    }
  ],
  "clientContext": "{\"guid\":\"b92\",\"hostname\":\"test.test.org\",\"ac2\":1}",
  "expirationMillis": 1898103480266,
  "status": 0,
  "totalCount": 1,
  "uId": "103299"
}
```

## Topics

### Request and Response

object GetVppAssetRequest

The request for an asset.

object GetVppAssetResponse

The response with the asset.

## See Also

### Asset and License Management

Get Assignments

Get a list of assignments currently assigned to a user or device.

Deprecated

Get Licenses

Get the set of licenses managed by your organization.

Deprecated

Manage Licenses

Associate and disassociate licenses with users and devices.

Deprecated

