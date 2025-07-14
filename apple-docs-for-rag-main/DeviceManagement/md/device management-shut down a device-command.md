

- Device Management
-  Shut Down a Device 

Web Service Endpoint

# Shut Down a Device

Remotely and immediately shut down a device.

iOS 10.3+iPadOS 10.3+macOS 10.13+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ShutDownDeviceCommand
```

## HTTP Body

ShutDownDeviceCommand

The command to shut down a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ShutDownDeviceResponse

`OK`

A response from the device after it processes the command to shut down.

Content-Type: application/xml

## Discussion

A passcode-locked iOS device doesn’t rejoin a Wi-Fi network after restarting, so it may not be able to communicate with the server.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                             |
|----------------------------|-----------------------------|
| Device Channel             | iOS, macOS, Shared iPad     |
| User Channel               | \-                          |
| Requires Supervision       | iOS                         |
| Allowed in User Enrollment | \-                          |
| Required Access Right      | AllowPasscodeRemovalAndLock |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        ShutDownDevice

    CommandUUID
    0001_ShutDownDevice

```

```

    CommandUUID
    0001_ShutDownDevice
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ShutDownDeviceCommand

The command to shut down a device.

object ShutDownDeviceResponse

A response from the device after it processes the command to shut down.

## See Also

### Device State

Erase a Device

Remotely and immediately erase a device.

Lock a Device

Remotely and immediately lock a device.

Restart a Device

Remotely and immediately restart a device.

