

- Device Management
-  Client Config 

Web Service Endpoint

# Client Config

Store client-specific information on the server.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/v2/client/config
```

## HTTP Body

ClientConfigRequest

missing

Content-Type: application/json

## Response Codes

` 200 ``OK`

ClientConfigResponse

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

Managing Users

Subscribing to Notifications

Managing Apps and Books Through Web Services

Managing Assets

## Discussion

### Example Request and Response

- Request
- Response

```
{
    "mdmInfo": {
        "id": "522d5c43-44ca-4f7e-ba7a-53570cf60765",
        "name": "Apple Configurator 2",
        "metadata": "2.13.3"
    },
    "notificationAuthToken": "SUp3rS3Cr3t",
    "notificationUrl": "https://www.next.com/notification",
    "notificationTypes": [
        "ASSET_COUNT",
        "ASSET_MANAGEMENT",
        "USER_MANAGEMENT",
        "USER_ASSOCIATED"
    ]
}
```

```
{
    "countryISO2ACode": "US",
    "defaultPlatform": "volumestore",
    "locationName": "PS01",
    "mdmInfo": {
        "id": "522d5c43-44ca-4f7e-ba7a-53570cf60765", 
        "name": "Apple Configurator 2", 
        "metadata": "2.13.3"
    },
    "notificationAuthToken": "SUp3rS3Cr3t",
    "notificationUrl": "https://www.next.com/notification",
    "subscribedNotificationTypes": [
        "ASSET_COUNT",
        "ASSET_MANAGEMENT",
        "USER_MANAGEMENT",
        "USER_ASSOCIATED"
    ],
    "tokenExpirationDate": "2030-11-08T22:33:22+0000",
    "uId": "2049025000431439",
    "websiteURL": "https://school.apple.com"
}
```

## Topics

### Request and Response

object ClientConfigRequest

The request for the client configuration.

object ClientConfigResponse

The response that contains the client configuration.

object ErrorResponse

The response that contains the error that occurs.

### Read-Only

Client Config

Read client-specific information from the server.

## See Also

### Configuration Management

Service Config

Provides the full list of web service URLs, notification types, request limits, and possible error codes.

