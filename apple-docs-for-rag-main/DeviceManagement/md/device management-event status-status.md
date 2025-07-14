

- Device Management
-  Event Status 

Web Service Endpoint

# Event Status

Retrieve the status of an asynchronous event.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://vpp.itunes.apple.com/mdm/v2/status
```

## Query Parameters

`eventId`

`string`

The unique identifier for the asynchronous event.

## Response Codes

` 200 ``OK`

StatusResponse

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

Managing Users

Handling Error Responses

Managing Assets

## Discussion

### Example Request and Response

- Request
- Response

```
?eventId=1905643d-1afb-4c2d-ad74-1b268e92c880
```

```
{
    "eventStatus": "COMPLETE",
    "eventType": "ASSOCIATE",
    "numCompleted": 4000,
    "numRequested": 4000,
    "tokenExpirationDate": "2030-11-08T22:33:22+0000",
    "uId": "2049025000431439"
}
```

## Topics

### Response

object StatusResponse

The response that contains the event status.

object ErrorResponse

The response that contains the error that occurs.

