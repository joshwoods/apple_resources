

- Device Management
-  LOM Device Request Command 

Web Service Endpoint

# LOM Device Request Command

Send requests to a device using lights-out management (LOM).

macOS 11.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#LOMDeviceRequestCommand
```

## HTTP Body

LOMDeviceRequestCommand

The command to send requests to a device using lights-out management (LOM).

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

LOMDeviceRequestResponse

`OK`

A response from the device after it processes requests it receives through lights-out management (LOM).

Content-Type: application/xml

## Discussion

This command requires the `DeviceLockAndRemovePasscode` access right, LightsOutManagementLOM configuration and is available in macOS 11 and later on supported macOS devices.

`DeviceDNSName` is the `CommonName` in the Identity issued on the client certificate from LightsOutManagementLOM. LOMSetupRequestResponse returns `PrimaryIPv6AddressList` and `SecondaryIPv6AddressList` after a successful deployment of Lights Out management configuration payload and subsequent LOMSetupRequestCommand.

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

        RequestList

            DeviceDNSName
            lomdevice.com
            DeviceRequestType
            Reset
            DeviceRequestUUID
            0001
            PrimaryIPv6AddressList

                fe80::94f6:d6ff:fef3:c05b
                fe80::94f6:d6ff:fef3:c1a4

            SecondaryIPv6AddressList

    CommandUUID
    0001_LOMDeviceRequest

```

```

    CommandUUID
    0001_LOMDeviceRequest
    ResponseData

            DeviceRequestSucess

            DeviceRequestUUID
            0001

    Status
    Acknowledged
    UDID
    37CECCAB-99C1-5ADF-8A9A-2AFA3B6387B5

```

## Topics

### Command and Response

object LOMDeviceRequestCommand

The command to send requests to a device using lights-out management (LOM).

object LOMDeviceRequestResponse

A response from the device after it processes requests it receives through lights-out management (LOM).

## See Also

### Lights-Out Management

LOM Setup Request Command

Get information from a device to set up lights-out management (LOM).

