

- Device Management
-  Clear the Bypass Code for Activation Lock 

Web Service Endpoint

# Clear the Bypass Code for Activation Lock

Clear the Activation Lock bypass code on a device.

iOS 7.1+iPadOS 7.1+macOS 10.15+visionOS 2.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ClearActivationLockBypassCodeCommand
```

## HTTP Body

ClearActivationLockBypassCodeCommand

The command to clear the Activation Lock bypass code on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ClearActivationLockBypassCodeResponse

`OK`

A response from the device after it processes the command to clear the Activation Lock bypass code.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

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
        ClearActivationLockBypassCode

    CommandUUID
    0001_ClearActivationLockBypassCode

```

```

    CommandUUID
    0001_ClearActivationLockBypassCode
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ClearActivationLockBypassCodeCommand

The command to clear the Activation Lock bypass code on a device.

object ClearActivationLockBypassCodeResponse

A response from the device after it processes the command to clear the Activation Lock bypass code.

## See Also

### Security

Security Information

Get security-related information about a device.

List the Certificates

Get a list of installed certificates on a device.

Get the Bypass Code for Activation Lock

Get the code to bypass Activation Lock on a device.

Rotate the FileVault Key

Change the FileVault primary password on a device.

