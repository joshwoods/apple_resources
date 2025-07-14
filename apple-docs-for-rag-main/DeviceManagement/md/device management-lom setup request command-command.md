

- Device Management
-  LOM Setup Request Command 

Web Service Endpoint

# LOM Setup Request Command

Get information from a device to set up lights-out management (LOM).

macOS 11.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#LOMSetupRequestCommand
```

## HTTP Body

LOMSetupRequestCommand

The command to get information from a device to set up lights-out management (LOM).

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

LOMSetupRequestResponse

`OK`

A response from the device after it processes the command to get setup information for lights-out management (LOM).

Content-Type: application/xml

## Discussion

This command requires the `DeviceLockAndRemovePasscode` access right, LightsOutManagementLOM configuration and is available in macOS 11 and later on supported macOS devices.

### Command Availability

|                            |                             |
|----------------------------|-----------------------------|
| Device Channel             | macOS                       |
| User Channel               | \-                          |
| Requires Supervision       | \-                          |
| Allowed in User Enrollment | \-                          |
| Required Access Right      | DeviceLockAndRemovePasscode |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        LOMSetupRequest

    CommandUUID
    0001_LOMSetupRequest

```

```

    CommandUUID
    0001_LOMSetupRequest
    PrimaryIPv6AddressList

       fe80::94f6:d6ff:fef3:c05b
       fe80::94f6:d6ff:fef3:c1a4

    Status
    Acknowledged
    UDID
    84341F79-92F5-5EF7-9A6A-3A7374613227

```

## Topics

### Command and Response

object LOMSetupRequestCommand

The command to get information from a device to set up lights-out management (LOM).

object LOMSetupRequestResponse

A response from the device after it processes the command to get setup information for lights-out management (LOM).

## See Also

### Lights-Out Management

LOM Device Request Command

Send requests to a device using lights-out management (LOM).

