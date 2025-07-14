

- Device Management
-  Start AirPlay Mirroring 

Web Service Endpoint

# Start AirPlay Mirroring

Prompt the user to share their screen using AirPlay Mirroring.

iOS 7.0+iPadOS 7.0+macOS 10.10+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#RequestMirroringCommand
```

## HTTP Body

RequestMirroringCommand

The command to prompt the user to share their screen using AirPlay Mirroring.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

RequestMirroringResponse

`OK`

A response from the device after it processes the command to prompt the user to share their screen using AirPlay Mirroring.

Content-Type: application/xml

## Discussion

MDM doesn’t support AirPlay destinations that have enabled Onscreen Codes. Provide either the `DestinationName` or the `DestinationDeviceID`. If you provide both values, MDM uses `DestinationDeviceID`.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS, macOS, Shared iPad |
| User Channel               | macOS                   |
| Requires Supervision       | \-                      |
| Allowed in User Enrollment | iOS, macOS              |
| Required Access Right      | \-                      |

### Example Request and Response

- Request
- Response

```

    Command

        DestinationName
        Apple TV
        Password
        password
        RequestType
        RequestMirroring
        ScanTime
        30

    CommandUUID
    0001_RequestMirroring

```

```

    CommandUUID
    0001_RequestMirroring
    MirroringResult
    Unknown
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object RequestMirroringCommand

The command to prompt the user to share their screen using AirPlay Mirroring.

object RequestMirroringResponse

A response from the device after it processes the command to prompt the user to share their screen using AirPlay Mirroring.

## See Also

### AirPlay Mirroring

Stop AirPlay Mirroring

Stop mirroring the display on another device.

