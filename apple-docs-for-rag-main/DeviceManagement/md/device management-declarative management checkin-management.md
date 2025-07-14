

- Device Management
-  Declarative Management Checkin 

Web Service Endpoint

# Declarative Management Checkin

The checkin protocol for declarative management.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#DeclarativeManagementRequest
```

## HTTP Body

DeclarativeManagementRequest

A checkin request that supports synchronization of declarations and status reports.

Content-Type: application/x-apple-aspen-mdm-checkin

## Response Codes

` 200 ``OK`

`OK`

## Mentioned in 

Integrating Declarative Management

## Topics

### Requests

object DeclarativeManagementRequest

The declarative managmement request details.

## See Also

### Declarative Management

Get Server Supported Declarations

Get a list of the declarations available on the server.

Get the Device Status

The request for getting the status of a device.

Get the Device Token

The request for sending the device token details.

