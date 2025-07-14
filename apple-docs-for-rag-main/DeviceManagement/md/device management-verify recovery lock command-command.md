

- Device Management
-  Verify Recovery Lock Command 

Web Service Endpoint

# Verify Recovery Lock Command

Verify the device’s Recovery Lock password.

macOS 11.5+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#VerifyRecoveryLockCommand
```

## HTTP Body

VerifyRecoveryLockCommand

The command to verify the password for Recovery Lock.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

VerifyRecoveryLockResponse

`OK`

A response from the device after it verifies the password for Recovery Lock.

Content-Type: application/xml

## Discussion

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
        VerifyRecoveryLock
        Password
        Apple

```

```

    CommandUUID
    0001_VerifyRecoveryLock
    PasswordVerified

    Status
    Acknowledged
    UDID
    1AC99473-AE6F-5E59-BE5C-410D257D481E

```

## Topics

### Command and Response

object VerifyRecoveryLockCommand

The command to verify the password for Recovery Lock.

object VerifyRecoveryLockResponse

A response from the device after it verifies the password for Recovery Lock.

## See Also

### Recovery Lock

Set Recovery Lock Command

Set or clear the Recovery Lock password.

