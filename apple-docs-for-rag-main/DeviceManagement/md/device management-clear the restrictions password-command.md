

- Device Management
-  Clear the Restrictions Password 

Web Service Endpoint

# Clear the Restrictions Password

Clear the restrictions password and the restrictions on a device.

iOS 8.0+iPadOS 8.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ClearRestrictionsPasswordCommand
```

## HTTP Body

ClearRestrictionsPasswordCommand

The command to clear the restrictions passcode on a device to disable or edit parental controls.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ClearRestrictionsPasswordResponse

`OK`

A response from the device after it processes the command to clear the restrictions password and the restrictions on a device.

Content-Type: application/xml

## Discussion

In iOS 11 and earlier, this command clears the restrictions password and all restrictions that the password protects.

In iOS 12.2 and later, if Screen Time uses iCloud to share its settings (Share Across Devices), this command disables Screen Time entirely and clears its restrictions. If the user is a child in an iCloud family, the command fails. Otherwise, if Screen Time isn’t using iCloud, this command clears the passcode, but not the restrictions, and it leaves Screen Time enabled.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |     |
|----------------------------|-----|
| Device Channel             | iOS |
| User Channel               | \-  |
| Requires Supervision       | iOS |
| Allowed in User Enrollment | \-  |
| Required Access Right      | \-  |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        ClearRestrictionsPassword

    CommandUUID
    0001_ClearRestrictionsPassword

```

```

    CommandUUID
    0001_ClearRestrictionsPassword
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ClearRestrictionsPasswordCommand

The command to clear the restrictions passcode on a device to disable or edit parental controls.

object ClearRestrictionsPasswordResponse

A response from the device after it processes the command to clear the restrictions password and the restrictions on a device.

## See Also

### Passwords

Clear the Passcode

Remove the passcode from a device.

Unlock a User Account

Unlock a user account that the system locked because of too many failed password attempts.

Set the Local Administrator Password

Update the local administrator account password.

Set the Firmware Password

Change or clear the firmware password on a device.

Verify the Firmware Password

Verify the firmware password on a device.

