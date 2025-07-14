

- Device Management
-  Invite to the Program 

Web Service Endpoint

# Invite to the Program

Invite a user to join the Volume Purchase Program (VPP).

iOS 7.0+iPadOS 7.0+macOS 10.9+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#InviteToProgramCommand
```

## HTTP Body

InviteToProgramCommand

The command to invite a user on a device to join the Volume Purchase Program (VPP).

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

InviteToProgramResponse

`OK`

A response from the device after it processes the command to invite a user to join the Volume Purchase Program (VPP).

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | Shared iPad, macOS                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | \-                                     |
| Required Access Right      | AllowAppInstallation                   |

### Example Request and Response

- Request
- Response

```

    Command

        InvitationURL
        https://buy.itunes.apple.com/WebObjects/MZFinance.woa/wa/associateVPPUserWithITSAccount?cc=us&amp;inviteCode=7770596534cf46b58fb0254e7112a5e5&amp;mt=8
        ProgramID
        com.apple.cloudvpp
        RequestType
        InviteToProgram

    CommandUUID
    0001_InviteToProgram

```

```

    CommandUUID
    0001_InviteToProgram
    InvitationResult
    Acknowledged
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object InviteToProgramCommand

The command to invite a user on a device to join the Volume Purchase Program (VPP).

object InviteToProgramResponse

A response from the device after it processes the command to invite a user to join the Volume Purchase Program (VPP).

## See Also

### Accounts

Account Configuration

Create and configure a local administrator account on a device.

