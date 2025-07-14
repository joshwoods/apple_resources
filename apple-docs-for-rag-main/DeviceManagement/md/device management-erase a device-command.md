

- Device Management
-  Erase a Device 

Web Service Endpoint

# Erase a Device

Remotely and immediately erase a device.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#EraseDeviceCommand
```

## HTTP Body

EraseDeviceCommand

The command to erase a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

EraseDeviceResponse

`OK`

A response from the device after it processes the command to erase.

Content-Type: application/xml

## Discussion

This command allows the server to immediately erase a device, even a locked device, without warning the user. The device sends a response to the server, but it doesn’t retry if it isn’t successful the first time.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | \-                                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | \-                                     |
| Required Access Right      | AllowDeviceErase                       |

### Example Request and Response

- Request
- Response

```

    Command

        DisallowProximitySetup

        PreserveDataPlan

        RequestType
        EraseDevice

    CommandUUID
    0001_EraseDevice

```

```

    CommandUUID
    0001_EraseDevice
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object EraseDeviceCommand

The command to erase a device.

object EraseDeviceResponse

A response from the device after it processes the command to erase.

## See Also

### Device State

Lock a Device

Remotely and immediately lock a device.

Restart a Device

Remotely and immediately restart a device.

Shut Down a Device

Remotely and immediately shut down a device.

