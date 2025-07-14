

- Device Management
-  Restart a Device 

Web Service Endpoint

# Restart a Device

Remotely and immediately restart a device.

iOS 10.3+iPadOS 10.3+macOS 10.13+tvOS 10.2+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#RestartDeviceCommand
```

## HTTP Body

RestartDeviceCommand

The command to restart a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

RestartDeviceResponse

`OK`

A response from the device after it processes the command to restart.

Content-Type: application/xml

## Discussion

A passcode-locked iOS device doesn’t rejoin a Wi-Fi network after restarting, so it may not be able to communicate with the server.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                               |
|----------------------------|-------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS |
| User Channel               | \-                            |
| Requires Supervision       | iOS, tvOS                     |
| Allowed in User Enrollment | \-                            |
| Required Access Right      | AllowPasscodeRemovalAndLock   |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        RestartDevice

    CommandUUID
    0001_RestartDevice

```

```

    CommandUUID
    0001_RestartDevice
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object RestartDeviceCommand

The command to restart a device.

object RestartDeviceResponse

A response from the device after it processes the command to restart.

## See Also

### Device State

Erase a Device

Remotely and immediately erase a device.

Lock a Device

Remotely and immediately lock a device.

Shut Down a Device

Remotely and immediately shut down a device.

