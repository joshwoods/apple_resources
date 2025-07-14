

- Device Management
-  Get the Bypass Code for Activation Lock 

Web Service Endpoint

# Get the Bypass Code for Activation Lock

Get the code to bypass Activation Lock on a device.

iOS 7.1+iPadOS 7.1+macOS 10.15+visionOS 2.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ActivationLockBypassCodeCommand
```

## HTTP Body

ActivationLockBypassCodeCommand

The command to get the code to bypass Activation Lock on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ActivationLockBypassCodeResponse

`OK`

A response from the device after it processes the command to get the Activation Lock bypass code.

Content-Type: application/xml

## Mentioned in 

Creating and Using Bypass Codes

## Discussion

iOS 7.1 adds support for bypassing Activation Lock. This allows organizations to remove the Activation Lock from supervised devices prior to device activation without knowing the userʼs personal Apple ID and password. Use this command to retrieve the device’s bypass code.

When an iOS device is a supervised device, it generates a device-specific Activation Lock bypass code. The activation server verifies this code to bypass Activation Lock on the device. For more information, see Creating and Using Bypass Codes.

A device creates a new bypass code when:

- Setting up the device the first time.

- Erasing and not restoring the device from a backup.

- Erasing and restoring the device from a backup from a different device.

### Query Availability

|                            |            |
|----------------------------|------------|
| Device Channel             | iOS, macOS |
| User Channel               | \-         |
| Requires Supervision       | iOS, macOS |
| Allowed in User Enrollment | \-         |
| Required Access Right      | \-         |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        ActivationLockBypassCode

    CommandUUID
    0001_ActivationLockBypassCode

```

```

    ActivationLockBypassCode
    A8QK7-GFG21-6RHT-V0U9-756P-L7E3
    CommandUUID
    0001_ActivationLockBypassCode
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ActivationLockBypassCodeCommand

The command to get the code to bypass Activation Lock on a device.

object ActivationLockBypassCodeResponse

A response from the device after it processes the command to get the Activation Lock bypass code.

## See Also

### Security

Security Information

Get security-related information about a device.

List the Certificates

Get a list of installed certificates on a device.

Clear the Bypass Code for Activation Lock

Clear the Activation Lock bypass code on a device.

Rotate the FileVault Key

Change the FileVault primary password on a device.

