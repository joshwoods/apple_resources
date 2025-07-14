

- Device Management
-  Get Assignments 

Web Service Endpoint

# Get Assignments

Get the set of current assignments for users or devices.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://vpp.itunes.apple.com/mdm/v2/assignments
```

## Query Parameters

`adamId`

`string`

The filter for the assignment product’s unique identifier.

`clientUserId`

`string`

The filter for the unique identifier of assigned users in your organization.

`pageIndex`

`int32`

The requested page index.

`serialNumber`

`string`

The filter for the unique identifier of assigned devices in your organization.

`sinceVersionId`

`string`

The filter for modified assignments since the specified version identifier.

## Response Codes

` 200 ``OK`

GetAssignmentsResponse

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

Managing Apps and Books Through Web Services

Upgrading to the new App and Book Management API

Using Paginated Endpoints

Managing Assets

## Discussion

### Example Request and Response

- Request
- Response

```
?adamId=408709785
```

```
{
    "assignments": [
        {
            "adamId": "408709785",
            "clientUserId": "client-1",
            "pricingParam": "STDQ"
        },
        {
            "adamId": "408709785",
            "serialNumber": "serial-1",
            "pricingParam": "STDQ"
        }
    ],
    "size": 2,
    "currentPageIndex": 0,
    "tokenExpirationDate": "2030-11-08T22:33:22+0000",
    "totalPages": 1,
    "uId": "2049025000431439",
    "versionId": "009061cb-87d1-4ea8-ae4c-7849dc49224e"
}
```

## Topics

### Response

object GetAssignmentsResponse

The paginated response that contains requested assignments.

object ErrorResponse

The response that contains the error that occurs.

## See Also

### Asset Management

Get Assets

Get the set of assets that your organization manages.

Associate Assets

Associate assets with client user IDs and serial numbers.

Disassociate Assets

Disassociate assets from client user IDs and serial numbers.

Revoke Assets

Revoke assets from client user IDs and serial numbers.

