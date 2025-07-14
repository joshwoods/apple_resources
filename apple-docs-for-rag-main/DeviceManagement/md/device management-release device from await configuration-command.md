

- Device Management
-  Release Device from Await Configuration 

Web Service Endpoint

# Release Device from Await Configuration

Inform the device that it can allow the user to continue in Setup Assistant.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 10.2+visionOS 2.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#DeviceConfiguredCommand
```

## HTTP Body

DeviceConfiguredCommand

The command to inform a device that it can allow the user to continue in Setup Assistant.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

DeviceConfiguredResponse

`OK`

A response from the device after it processes the command to allow the user to continue in Setup Assistant.

Content-Type: application/xml

## Discussion

This command only works on Device Enrollment Program (DEP) devices that have their cloud configuration set to await configuration.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                               |
|----------------------------|-------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS |
| User Channel               | macOS, Shared iPad            |
| Requires Supervision       | \-                            |
| Allowed in User Enrollment | \-                            |
| Required Access Right      | \-                            |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        DeviceConfigured

    CommandUUID
    0001_DeviceConfigured

```

```

    CommandUUID
    0001_DeviceConfigured
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object DeviceConfiguredCommand

The command to inform a device that it can allow the user to continue in Setup Assistant.

object DeviceConfiguredResponse

A response from the device after it processes the command to allow the user to continue in Setup Assistant.

## See Also

### Device Details

List the Installed Apps

Get a list of the installed apps on a device.

Get Device Information

Get detailed information about a device.

User Configured Command

Informs the device that it can continue past Setup Assistant and finish login.

List the Installed Restrictions

Get a list of restrictions on the device.

