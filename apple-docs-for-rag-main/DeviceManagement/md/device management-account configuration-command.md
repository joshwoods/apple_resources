

- Device Management
-  Account Configuration 

Web Service Endpoint

# Account Configuration

Create and configure a local administrator account on a device.

macOS 10.11+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#AccountConfigurationCommand
```

## HTTP Body

AccountConfigurationCommand

The command to create a local administrator account on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

AccountConfigurationResponse

`OK`

A response from the device after it processes the command to create and configure a local administrator account.

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

        AutoSetupAdminAccounts

                fullName
                Administrator
                hidden

                shortName
                admin
                passwordHash

                    PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4K
                    PCFET0NUWVBFIHBsaXN0IFBVQkxJQyAiLS8vQXBwbGUvL0RURCBQ
                    TElTVCAxLjAvL0VOIiAiaHR0cDovL3d3dy5hcHBsZS5jb20vRFRE
                    cy9Qcm9wZXJ0eUxpc3QtMS4wLmR0ZCI+CjxwbGlzdCB2ZXJzaW9u
                    PSIxLjAiPgo8ZGljdD4KCTxrZXk+U0FMVEVELVNIQTUxMi1QQktE
                    RjI8L2tleT4KCTxkaWN0PgoJCTxrZXk+ZW50cm9weTwva2V5PgoJ
                    CTxkYXRhPgoJCXJiSXZtVGlQQlJ3cWZ6dmFQQnhPT1VLRHVnTnRM
                    YVVQZ2lIVnpBUWNsNDNjSmUzaGZ6ZW05TDVhczAyRQoJCXp2TEFl
                    aTJFT0tqMFNaOENpKzNXV0tQN2orMklSdWU0T1ZyTzBsYnhGOHR5
                    K3pZb0hTMTVRU3hGcUplagoJCU5qdkk1NTk1N1JjZUVLaXFSRjZ1
                    UEpQUTYvbUxEc0xnSTR4dko3NVpEa0JlYW51QkI0TT0KCQk8L2Rh
                    dGE+CgkJPGtleT5zYWx0PC9rZXk+CgkJPGRhdGE+CgkJTXVpS2g1
                    MjR3QkJMV0ZoQ3lzRFIzRnJPOGM0WlFIUGZTRE5JbDZvQjlCST0K
                    CQk8L2RhdGE+CgkJPGtleT5pdGVyYXRpb25zPC9rZXk+CgkJPGlu
                    dGVnZXI+NDAwMDA8L2ludGVnZXI+Cgk8L2RpY3Q+CjwvZGljdD4K
                    PC9wbGlzdD4K

        DontAutoPopulatePrimaryAccountInfo

        LockPrimaryAccountInfo

        PrimaryAccountFullName
        User
        PrimaryAccountUserName
        user
        RequestType
        AccountConfiguration
        SetPrimarySetupAccountAsRegularUser

        SkipPrimarySetupAccountCreation

    CommandUUID
    0001_AccountConfiguration

```

```

    CommandUUID
    0001_AccountConfiguration
    Status
    Acknowledged
    UDID
    91FE0F6E-F91C-589A-95E6-02835CE7126D

```

## Topics

### Command and Response

object AccountConfigurationCommand

The command to create a local administrator account on a device.

object AccountConfigurationResponse

A response from the device after it processes the command to create and configure a local administrator account.

## See Also

### Accounts

Invite to the Program

Invite a user to join the Volume Purchase Program (VPP).

