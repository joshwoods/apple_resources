

- Device Management
-  Associate Assets 

Web Service Endpoint

# Associate Assets

Associate assets with client user IDs and serial numbers.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/v2/assets/associate
```

## HTTP Body

ManageAssetsRequest

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

## Mentioned in 

Upgrading to the new App and Book Management API

## Discussion

### Example Request and Response

- Request
- Response

```
{
    "assets": [
        {
            "adamId": "408709785",
            "pricingParam": "STDQ"
        },
        {
            "adamId": "377298193",
            "pricingParam": "STDQ"
        }
    ],
    "clientUserIds": [
        "client-1",
        "client-2"
    ],
    "serialNumbers": [
        "serial-1",
        "serial-2"
    ]
}
```

```
```

## Topics

### Request and Response

object ManageAssetsRequest

The request for asset management.

object EventResponse

The response that contains the event identifier.

object ErrorResponse

The response that contains the error that occurs.

## See Also

### Asset Management

Get Assets

Get the set of assets that your organization manages.

Disassociate Assets

Disassociate assets from client user IDs and serial numbers.

Revoke Assets

Revoke assets from client user IDs and serial numbers.

Get Assignments

Get the set of current assignments for users or devices.

