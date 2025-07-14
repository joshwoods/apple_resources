

- Device Management
-  Set the Local Administrator Password 

Web Service Endpoint

# Set the Local Administrator Password

Update the local administrator account password.

macOS 10.11+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#SetAutoAdminPasswordCommand
```

## HTTP Body

SetAutoAdminPasswordCommand

The command to change the password of a local administrator account that Setup Assistant creates on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

SetAutoAdminPasswordResponse

`OK`

A response from the device after it processes the command to update the local administrator account password.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Requires Supervision       | macOS |
| Allowed in User Enrollment | \-    |
| Required Access Right      | \-    |

### Example Request and Response

- Request
- Response

```

    Command

        GUID
        F7C60A02-E0AB-4C87-8356-E0CC11568043
        RequestType
        SetAutoAdminPassword
        passwordHash

            PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4K
            PCFET0NUWVBFIHBsaXN0IFBVQkxJQyAiLS8vQXBwbGUvL0RURCBQ
            TElTVCAxLjAvL0VOIiAiaHR0cDovL3d3dy5hcHBsZS5jb20vRFRE
            cy9Qcm9wZXJ0eUxpc3QtMS4wLmR0ZCI+CjxwbGlzdCB2ZXJzaW9u
            PSIxLjAiPgo8ZGljdD4KCTxrZXk+U0FMVEVELVNIQTUxMi1QQktE
            RjI8L2tleT4KCTxkaWN0PgoJCTxrZXk+ZW50cm9weTwva2V5PgoJ
            CTxkYXRhPgoJCVpxcWVkTU5Ya3BtVjhEbU5iRFdUYjBHTDNSNjAz
            RHNVSllkb1BvV0NlK2gwRDNubC9mWCsxTlpKSUxPdgoJCTBxQTVC
            Q0FBSEZCZ3REQzVqeEF3a2NyZ1puZVd4eWpGZGpvT0hsV2RoYWVF
            T0MyaFBwVktIaC9WUk9uUQoJCXM2cWUvRGtaZ1djVDBQdk9VQ3NM
            ZVhTd2dOTU9UNGFwMnJWR0IxOVFwSFBpdnJrNmp2dz0KCQk8L2Rh
            dGE+CgkJPGtleT5pdGVyYXRpb25zPC9rZXk+CgkJPGludGVnZXI+
            NDAwMDA8L2ludGVnZXI+CgkJPGtleT5zYWx0PC9rZXk+CgkJPGRh
            dGE+CgkJZUl3Q3hxUk1NVm0wWGZ3VmpvbERCNEFUc2I0K3ZWMjdL
            Z1hDdU5ZMkNlOD0KCQk8L2RhdGE+Cgk8L2RpY3Q+CjwvZGljdD4K
            PC9wbGlzdD4K

    CommandUUID
    0001_SetAutoAdminPassword

```

```

    CommandUUID
    0001_SetAutoAdminPassword
    Status
    Acknowledged
    UDID
    91FE0F6E-F91C-589A-95E6-02835CE7126D

```

## Topics

### Command and Response

object SetAutoAdminPasswordCommand

The command to change the password of a local administrator account that Setup Assistant creates on a device.

object SetAutoAdminPasswordResponse

A response from the device after it processes the command to update the local administrator account password.

## See Also

### Passwords

Clear the Passcode

Remove the passcode from a device.

Clear the Restrictions Password

Clear the restrictions password and the restrictions on a device.

Unlock a User Account

Unlock a user account that the system locked because of too many failed password attempts.

Set the Firmware Password

Change or clear the firmware password on a device.

Verify the Firmware Password

Verify the firmware password on a device.

