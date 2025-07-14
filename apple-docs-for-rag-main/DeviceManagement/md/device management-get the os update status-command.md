

- Device Management
-  Get the OS Update Status 

Web Service Endpoint

# Get the OS Update Status

Get the status of operating-system updates on a device.

iOS 9.0+iPadOS 9.0+macOS 10.11.5+tvOS 12.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#OSUpdateStatusCommand
```

## HTTP Body

OSUpdateStatusCommand

The command to get the status of operating-system updates.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

OSUpdateStatusResponse

`OK`

A response from the device after it processes the command to get the status of operating-system updates.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Query Availability

|                            |                               |
|----------------------------|-------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS |
| User Channel               | \-                            |
| Requires Supervision       | iOS, macOS, tvOS              |
| Allowed in User Enrollment | \-                            |
| Required Access Right      | AllowAppInstallation          |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        OSUpdateStatus

    CommandUUID
    0001_OSUpdateStatus

```

```

    CommandUUID
    0001_OSUpdateStatus
    OSUpdateStatus

            DownloadPercentComplete
            0.5030184984207153
            IsDownloaded

            ProductKey
            iOSUpdate17A576
            Status
            Downloading

    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object OSUpdateStatusCommand

The command to get the status of operating-system updates.

object OSUpdateStatusResponse

A response from the device after it processes the command to get the status of operating-system updates.

## See Also

### Updates

Schedule an OS Update Scan

Schedule a background scan for operating-system updates on a device.

List the Available OS Updates

Get a list of available operating-system updates for a device.

Schedule an OS Update

Schedule an update of the operating system on a device.

