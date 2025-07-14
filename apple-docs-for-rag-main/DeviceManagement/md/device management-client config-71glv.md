

- Device Management
-  Client Config 

Web Service Endpoint

# Client Config

Read client-specific information from the server.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://vpp.itunes.apple.com/mdm/v2/client/config
```

## Response Codes

` 200 ``OK`

ClientConfigResponse

`OK`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorResponse

`Internal Server Error`

Content-Type: application/json

## Discussion

### Example Response

- Request
- Response

```
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

### Response

object ClientConfigResponse

The response that contains the client configuration.

object ErrorResponse

The response that contains the error that occurs.

