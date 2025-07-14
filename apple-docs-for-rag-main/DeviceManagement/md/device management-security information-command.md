

- Device Management
-  Security Information 

Web Service Endpoint

# Security Information

Get security-related information about a device.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#SecurityInfoCommand
```

## HTTP Body

SecurityInfoCommand

The command to get security-related information about a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

SecurityInfoResponse

`OK`

A response from the device after it processes the command to get security-related information.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Query Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | \-                                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Required Access Right      | AllowQuerySecurity                     |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        SecurityInfo

    CommandUUID
    0001_SecurityInfo

```

```

    CommandUUID
    0011_SecurityInfo
    SecurityInfo

        HardwareEncryptionCaps
        3
        ManagementStatus

            IsUserEnrollment

        PasscodeCompliant

        PasscodeCompliantWithProfiles

        PasscodeLockGracePeriod
        0
        PasscodeLockGracePeriodEnforced
        0
        PasscodePresent

    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object SecurityInfoCommand

The command to get security-related information about a device.

object SecurityInfoResponse

A response from the device after it processes the command to get security-related information.

## See Also

### Security

List the Certificates

Get a list of installed certificates on a device.

Get the Bypass Code for Activation Lock

Get the code to bypass Activation Lock on a device.

Clear the Bypass Code for Activation Lock

Clear the Activation Lock bypass code on a device.

Rotate the FileVault Key

Change the FileVault primary password on a device.

