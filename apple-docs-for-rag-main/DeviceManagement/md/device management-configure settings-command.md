

- Device Management
-  Configure Settings 

Web Service Endpoint

# Configure Settings

Configure settings on a device.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#SettingsCommand
```

## HTTP Body

SettingsCommand

The command to configure settings on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

SettingsResponse

`OK`

A response from the device after it processes the command to configure settings.

Content-Type: application/xml

## Discussion

Users may be able to change the settings later if a profile isn’t set to restrict such changes.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS, Shared iPad                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Required Access Right      | AllowSettings                          |

### Example Request and Response (DeviceName)

- Request
- Response

```

    Command

        RequestType
        Settings
        Settings

                DeviceName
                NewName
                Item
                DeviceName

    CommandUUID
    0001_Settings

```

```

    CommandUUID
    0001_Settings
    Settings

            Item
            DeviceName
            Status
            Acknowledged

    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object SettingsCommand

The command to configure settings on a device.

object SettingsResponse

A response from the device after it processes the command to configure settings on a device.

## See Also

### Managed Settings

Disable Remote Desktop

Disable Remote Desktop on a device.

Enable Remote Desktop

Enable Remote Desktop on a device.

