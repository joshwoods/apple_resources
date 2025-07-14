

- Device Management
-  Schedule an OS Update Scan 

Web Service Endpoint

# Schedule an OS Update Scan

Schedule a background scan for operating-system updates on a device.

macOS 10.11+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ScheduleOSUpdateScanCommand
```

## HTTP Body

ScheduleOSUpdateScanCommand

The command to schedule an operating-system update scan.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ScheduleOSUpdateScanResponse

`OK`

A response from the device after it processes the command to schedule an operating-system update scan.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Requires Supervision       | macOS |
| Allowed in User Enrollment | \-    |
| Required Access Right      | \-    |

### Example Request and Response

- Request
- Response

```

    Command

        ForceUpdateScan

        RequestType
        ScheduleOSUpdateScan

    CommandUUID
    0001_ScheduleOSUpdateScan

```

```

    CommandUUID
    0316_ScheduleOSUpdateScan
    ScanInitiated

    ScanInititated

    Status
    Acknowledged
    UDID
    E84CD517-CB37-52F7-988C-DB5137B604B8

```

## Topics

### Command and Response

object ScheduleOSUpdateScanCommand

The command to schedule an operating-system update scan.

object ScheduleOSUpdateScanResponse

A response from the device after it processes the command to schedule an operating-system update scan.

## See Also

### Updates

List the Available OS Updates

Get a list of available operating-system updates for a device.

Schedule an OS Update

Schedule an update of the operating system on a device.

Get the OS Update Status

Get the status of operating-system updates on a device.

