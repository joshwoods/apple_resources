

- Device Management
-  Disable Remote Desktop 

Web Service Endpoint

# Disable Remote Desktop

Disable Remote Desktop on a device.

macOS 10.14.4+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#DisableRemoteDesktopCommand
```

## HTTP Body

DisableRemoteDesktopCommand

The command to disable Remote Desktop on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

DisableRemoteDesktopResponse

`OK`

A response from the device after it processes the command to disable Remote Desktop.

Content-Type: application/xml

## Discussion

This command prevents any further event processing. It removes any `PostEvent` Transparency Consent and Control (TCC) ability, unless the device already has an installed TCC configuration profile with that ability enabled.

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
        DisableRemoteDesktop

    CommandUUID
    0001_DisableRemoteDesktop

```

```

    CommandUUID
    0001_DisableRemoteDesktop
    Status
    Acknowledged
    UDID
    E84CD517-CB37-52F7-988C-DB5137B604B8

```

## Topics

### Command and Response

object DisableRemoteDesktopCommand

The command to disable Remote Desktop on a device.

object DisableRemoteDesktopResponse

A response from the device after it processes the command to disable Remote Desktop.

## See Also

### Managed Settings

Enable Remote Desktop

Enable Remote Desktop on a device.

Configure Settings

Configure settings on a device.

