

- Device Management
-  Content Caching Information Command 

Web Service Endpoint

# Content Caching Information Command

Get the status of the content caches on a device.

macOS 10.15.4+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ContentCachingInformationCommand
```

## HTTP Body

ContentCachingInformationCommand

The command to get the status of the content caches on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ContentCachingInformationResponse

`OK`

A response from the device after it processes the command to get the status of the content caches on a device.

Content-Type: application/xml

## Topics

### Command and Response

object ContentCachingInformationCommand

The command to get the status of the content caches on a device.

object ContentCachingInformationResponse

A response from the device after it processes the command to get the status of the content caches on a device.

