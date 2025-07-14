

- Device Management
-  Verify the Firmware Password 

Web Service Endpoint

# Verify the Firmware Password

Verify the firmware password on a device.

macOS 10.13+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#VerifyFirmwarePasswordCommand
```

## HTTP Body

VerifyFirmwarePasswordCommand

The command to verify the firmware password on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

VerifyFirmwarePasswordResponse

`OK`

A response from the device after it processes the command to verify the firmware password.

Content-Type: application/xml

## Discussion

This command has a throttle interval to prevent executing it more frequently than every 30 seconds. Requests that occur within the throttle interval return an error.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

This command isn’t supported on Mac computers with Apple silicon.

### Command Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Requires Supervision       | \-    |
| Allowed in User Enrollment | \-    |
| Required Access Right      | \-    |

### Example Request and Response

- Request
- Response

```

    Command

        Password
        password
        RequestType
        VerifyFirmwarePassword

    CommandUUID
    0001_VerifyFirmwarePassword

```

```

    CommandUUID
    0001_VerifyFirmwarePassword
    Status
    Acknowledged
    UDID
    E84CD517-CB37-52F7-988C-DB5137B604B8
    VerifyFirmwarePassword

        PasswordVerified

```

## Topics

### Command and Response

object VerifyFirmwarePasswordCommand

The command to verify the firmware password on a device.

object VerifyFirmwarePasswordResponse

A response from the device after it processes the command to verify the firmware password.

## See Also

### Passwords

Clear the Passcode

Remove the passcode from a device.

Clear the Restrictions Password

Clear the restrictions password and the restrictions on a device.

Unlock a User Account

Unlock a user account that the system locked because of too many failed password attempts.

Set the Local Administrator Password

Update the local administrator account password.

Set the Firmware Password

Change or clear the firmware password on a device.

