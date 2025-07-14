

- Device Management
-  Stop AirPlay Mirroring 

Web Service Endpoint

# Stop AirPlay Mirroring

Stop mirroring the display on another device.

iOS 7.0+iPadOS 7.0+macOS 10.10+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#StopMirroringCommand
```

## HTTP Body

StopMirroringCommand

The command to stop mirroring the display on another device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

StopMirroringResponse

`OK`

A response from the device after it processes the command to stop mirroring the display on another device.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS, macOS, Shared iPad |
| User Channel               | \-                      |
| Requires Supervision       | iOS                     |
| Allowed in User Enrollment | \-                      |
| Required Access Right      | \-                      |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        StopMirroring

    CommandUUID
    0001_StopMirroring

```

```

    CommandUUID
    0001_StopMirroring
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object StopMirroringCommand

The command to stop mirroring the display on another device.

object StopMirroringResponse

A response from the device after it processes the command to stop mirroring the display on another device.

## See Also

### AirPlay Mirroring

Start AirPlay Mirroring

Prompt the user to share their screen using AirPlay Mirroring.

