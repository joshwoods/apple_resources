

- Device Management
-  Unlock a User Account 

Web Service Endpoint

# Unlock a User Account

Unlock a user account that the system locked because of too many failed password attempts.

macOS 10.13+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#UnlockUserAccountCommand
```

## HTTP Body

UnlockUserAccountCommand

The command to unlock a local user account on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

UnlockUserAccountResponse

`OK`

A response from the device after it processes the command to unlock a user account.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

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
        UnlockUserAccount
        UserName
        graham

    CommandUUID
    0001_UnlockUserAccount

```

```

    CommandUUID
    0001_UnlockUserAccount
    Status
    Acknowledged
    UDID
    91FE0F6E-F91C-589A-95E6-02835CE7126D

```

## Topics

### Command and Response

object UnlockUserAccountCommand

The command to unlock a local user account on a device.

object UnlockUserAccountResponse

A response from the device after it processes the command to unlock a user account.

## See Also

### Passwords

Clear the Passcode

Remove the passcode from a device.

Clear the Restrictions Password

Clear the restrictions password and the restrictions on a device.

Set the Local Administrator Password

Update the local administrator account password.

Set the Firmware Password

Change or clear the firmware password on a device.

Verify the Firmware Password

Verify the firmware password on a device.

