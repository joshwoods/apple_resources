

- Device Management
-  Get Assets 

Web Service Endpoint

# Get Assets

Get the set of assets that your organization manages.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://vpp.itunes.apple.com/mdm/v2/assets
```

## Query Parameters

`pageIndex`

`int32`

The requested page index.

`productType`

`string`

The filter for the asset product type.

Possible Values: `App, Book`

`pricingParam`

`string`

The filter for the asset product quality.

Possible Values: `STDQ, PLUS`

`revocable`

`boolean`

The filter for asset revocability.

`deviceAssignable`

`boolean`

The filter for asset device assignability.

`maxAvailableCount`

`int32`

The filter for the maximum inclusive assets available count.

`minAvailableCount`

`int32`

The filter for the minimum inclusive assets available count.

`maxAssignedCount`

`int32`

The filter for the maximum inclusive assets assigned count.

`minAssignedCount`

`int32`

The filter for the minimum inclusive assets assigned count.

`adamId`

`string`

The filter for the asset product unique identifier.

## Response Codes

` 200 ``OK`

GetAssetsResponse

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

## Mentioned in 

Using Paginated Endpoints

Managing Apps and Books Through Web Services

Upgrading to the new App and Book Management API

Managing Assets

## Discussion

### Example Request and Response

- Request
- Response

```
?pageIndex=0&pricingParam=STDQ&productType=App
```

```
{
    "assets": [
        {
            "adamId": "408709785",
            "assignedCount": 5000,
            "availableCount": 10000,
            "deviceAssignable": true,
            "pricingParam": "STDQ",
            "productType": "App",
            "retiredCount": 0,
            "revocable": true,
            "supportedPlatforms": ["iOS"],
            "totalCount": 15000
        },
        {
            "adamId": "377298193",
            "assignedCount": 5000,
            "availableCount": 10000,
            "deviceAssignable": true,
            "pricingParam": "STDQ",
            "productType": "App",
            "retiredCount": 0,
            "revocable": true,
            "supportedPlatforms": ["iOS"],
            "totalCount": 15000
        },
        {
            "adamId": "361309726",
            "assignedCount": 5000,
            "availableCount": 10000,
            "deviceAssignable": true,
            "pricingParam": "STDQ",
            "productType": "App",
            "retiredCount": 0,
            "revocable": true,
            "supportedPlatforms": ["iOS"],
            "totalCount": 15000
        },
        {
            "adamId": "361304891",
            "assignedCount": 5000,
            "availableCount": 10000,
            "deviceAssignable": true,
            "pricingParam": "STDQ",
            "productType": "App",
            "retiredCount": 0,
            "revocable": true,
            "supportedPlatforms": ["iOS"],
            "totalCount": 15000
        },
        {
            "adamId": "361285480",
            "assignedCount": 5000,
            "availableCount": 10000,
            "deviceAssignable": true,
            "pricingParam": "STDQ",
            "productType": "App",
            "retiredCount": 0,
            "revocable": true,
            "supportedPlatforms": ["iOS"],
            "totalCount": 15000
        }
    ],
    "currentPageIndex": 0,
    "size": 5,
    "tokenExpirationDate": "2030-11-08T22:33:22+0000",
    "totalPages": 1,
    "uId": "2049025000431439",
    "versionId": "70e8c740-514c-11eb-bb63-a90b882fcd52"
}
```

## Topics

### Response

object GetAssetsResponse

The paginated response that contains the requested assets.

object ErrorResponse

The response that contains the error that occurs.

### Content Metadata

Apps and Books for Organizations

Get details about apps and books to show to your users.

## See Also

### Asset Management

Associate Assets

Associate assets with client user IDs and serial numbers.

Disassociate Assets

Disassociate assets from client user IDs and serial numbers.

Revoke Assets

Revoke assets from client user IDs and serial numbers.

Get Assignments

Get the set of current assignments for users or devices.

