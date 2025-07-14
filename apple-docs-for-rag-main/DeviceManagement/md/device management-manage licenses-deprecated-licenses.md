

- Device Management
-  Manage Licenses Deprecated

Web Service Endpoint

# Manage Licenses

Associate and disassociate licenses with users and devices.

Device Assignment ServicesVPP License Management

Deprecated

This legacy API is currently in maintenance mode. Apple won’t add any new functionality to it.

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/manageVPPLicensesByAdamIdSrv
```

## HTTP Body

ManageVppLicensesByAdamIdRequest

missing

Content-Type: application/json

## Response Codes

` 200 ``OK`

ManageVppLicensesByAdamIdResponse

`OK`

Content-Type: application/json

## Discussion

This endpoint operates on a single asset (specified by the `{adamIdStr, pricingParam}` tuple) for multiple associations and disassociations in a single request.

Licenses are disassociated from all users specified by the `disassociateClientUserIdStrs` array, the devices specified by the `disassociateSerialNumbers` array, or the licenses specified by the `disassociateLicenseIdStrs` array (which must only specify licenses assigned to the specified asset). At most one of these `disassociate*` arrays may be specified per request.

Then licenses are associated either with the users specified by the `associateClientUserIdStrs` array or the devices specified by the `associateSerialNumbers` array. Device assignment doesn’t trigger notifcation.

At most, one `associate*` and one `disassociate*` array is allowed per request. Specifying more than one of either `associate*` or `disassociate*` arrays result in undefined behavior.

### Example Request and Response with a Serial Number

- Request
- Response

```
{
  "disassociateClientUserIdStrs": null,
  "disassociateSerialNumbers": null,
  "disassociateLicenseIdStrs": null,
  "associateClientUserIdStrs": null,
  "associateSerialNumbers": [
    "MERD1",
    "MERD2"
  ],
  "adamIdStr": "869183446",
  "pricingParam": null,
  "notifyDisassociation": true,
  "sToken": "h40Gte9aQnZFDNM39IUkRPCsQDxBxbZB4Wy34pxefOuQkeeb3h2 a5Rlopo4KDn3MrFKf4CM3OY+WGAoZ1cD6iZ6yzsMk1+5PVBNc66YS6ZQ="
}
```

```
{
  "adamIdStr": "869183446",
  "associations": [
    {
      "licenseIdStr": "840999",
      "serialNumber": "device1"
    },
    {
      "licenseIdStr": "841000",
      "serialNumber": "device1"
    }
  ],
  "clientContext": "{\"guid\":\"b92\",\"hostname\":\"test.test.org\",\"ac2\":1}",
  "expirationMillis": 1898103480266,
  "isIrrevocable": false,
  "location": {
    "locationId": 22222222222,
    "locationName": "LocationName"
  },
  "pricingParam": "STDQ",
  "productTypeId": 8,
  "productTypeName": "Application",
  "status": 0,
  "uId": "103614"
}
```

### Example Request and Response with a Client User ID String

- Request
- Response

```
{
  "disassociateClientUserIdStrs": null,
  "disassociateSerialNumbers": null,
  "disassociateLicenseIdStrs": null,
  "associateClientUserIdStrs": [
    "9a17b450-9820-471e-b232-13a479ddede0"
  ],
  "associateSerialNumbers": null,
  "adamIdStr": "869183446",
  "pricingParam": null,
  "notifyDisassociation": null,
  "sToken": "h40Gte9aQnZFDNM39IUkRPCsQDxBxbZB4Wy34pxefOuQkeeb3h2 a5Rlopo4KDn3MrFKf4CM3OY+WGAoZ1cD6iZ6yzsMk1+5PVBNc66YS6ZQ="
}
```

```
{
  "adamIdStr": "869183446",
  "associations": [
    {
      "licenseIdStr": "840998",
      "clientUserIdStr": "9a17b450-9820-471e-b232-13a479ddede0"
    }
  ],
  "clientContext": "{\"guid\":\"b92\",\"hostname\":\"test.test.org\",\"ac2\":1}",
  "expirationMillis": 1898103480266,
  "isIrrevocable": false,
  "location": {
    "locationId": 22222222222,
    "locationName": "LocationName"
  },
  "pricingParam": "STDQ",
  "productTypeId": 8,
  "productTypeName": "Application",
  "status": 0,
  "uId": "103614"
}
```

## Topics

### Request and Response

object ManageVppLicensesByAdamIdRequest

The request to manage licenses.

object ManageVppLicensesByAdamIdResponse

The response from managing licenses.

## See Also

### Asset and License Management

Get Assets

Get the set of assets managed by your organization.

Deprecated

Get Assignments

Get a list of assignments currently assigned to a user or device.

Deprecated

Get Licenses

Get the set of licenses managed by your organization.

Deprecated

