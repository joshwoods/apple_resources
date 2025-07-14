

- Device Management
-  Get the Device Status 

Web Service Endpoint

# Get the Device Status

The request for getting the status of a device.

Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#status
```

## HTTP Body

StatusReport

A status report of the device’s current state.

Content-Type: application/json

## Response Codes

` 204 ``No Content`

`No Content`

## See Also

### Declarative Management

Declarative Management Checkin

The checkin protocol for declarative management.

Get Server Supported Declarations

Get a list of the declarations available on the server.

Get the Device Token

The request for sending the device token details.

