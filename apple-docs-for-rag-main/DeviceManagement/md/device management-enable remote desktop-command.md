

- Device Management
-  Enable Remote Desktop 

Web Service Endpoint

# Enable Remote Desktop

Enable Remote Desktop on a device.

macOS 10.14.4+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#EnableRemoteDesktopCommand
```

## HTTP Body

EnableRemoteDesktopCommand

The command to enable Remote Desktop on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

EnableRemoteDesktopResponse

`OK`

A response from the device after it processes the command to enable Remote Desktop.

Content-Type: application/xml

## Discussion

This command enables the following capabilities on the device:

- Remote Desktop with the All Users access

- The ability to receive remote events

- The Observe, Control, and Show being Observed options

All other options remain unchanged.

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

        RequestType
        EnableRemoteDesktop

    CommandUUID
    0001_EnableRemoteDesktop

```

```

    CommandUUID
    0001_EnableRemoteDesktop
    Status
    Acknowledged
    UDID
    E84CD517-CB37-52F7-988C-DB5137B604B8

```

## Topics

### Command and Response

object EnableRemoteDesktopCommand

The command to enable Remote Desktop on a device.

object EnableRemoteDesktopResponse

A response from the device after it processes the command to enable Remote Desktop on a device.

## See Also

### Managed Settings

Disable Remote Desktop

Disable Remote Desktop on a device.

Configure Settings

Configure settings on a device.

