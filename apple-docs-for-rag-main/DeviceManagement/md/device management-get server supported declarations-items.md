

- Device Management
-  Get Server Supported Declarations 

Web Service Endpoint

# Get Server Supported Declarations

Get a list of the declarations available on the server.

Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#declaration-items
```

## Response Codes

` 200 ``OK`

DeclarationItemsResponse

`OK`

Content-Type: application/json

## Topics

### Response

object DeclarationItemsResponse

The set of available declarations on the server.

## See Also

### Declarative Management

Declarative Management Checkin

The checkin protocol for declarative management.

Get the Device Status

The request for getting the status of a device.

Get the Device Token

The request for sending the device token details.

