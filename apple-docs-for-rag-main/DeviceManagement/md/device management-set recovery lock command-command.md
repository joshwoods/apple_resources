

- Device Management
-  Set Recovery Lock Command 

Web Service Endpoint

# Set Recovery Lock Command

Set or clear the Recovery Lock password.

macOS 11.5+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#SetRecoveryLockCommand
```

## HTTP Body

SetRecoveryLockCommand

The command to set the password for Recovery Lock.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

SetRecoveryLockResponse

`OK`

A response from the device after it sets the password for Recovery Lock.

Content-Type: application/xml

## Discussion

This command sets, or clears, a password on booting to recoveryOS. When the device unenrolls MDM the system removes the recovery password.

This command is only available with Apple silicon.

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
        SetRecoveryLock
        NewPassword
        Apple

```

```

    CommandUUID
    0001_SetRecoveryLock
    Status
    Acknowledged
    UDID
    1AC99473-AE6F-5E59-BE5C-410D257D481E

```

## Topics

### Command and Response

object SetRecoveryLockCommand

The command to set the password for Recovery Lock.

object SetRecoveryLockResponse

A response from the device after it sets the password for Recovery Lock.

## See Also

### Recovery Lock

Verify Recovery Lock Command

Verify the device’s Recovery Lock password.

