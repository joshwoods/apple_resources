

- Device Management
-  Rotate the FileVault Key 

Web Service Endpoint

# Rotate the FileVault Key

Change the FileVault primary password on a device.

macOS 10.9+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#RotateFileVaultKeyCommand
```

## HTTP Body

RotateFileVaultKeyCommand

The command to change the FileVault primary password on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

RotateFileVaultKeyResponse

`OK`

A response from the device after it processes the command to change the FileVault primary password.

Content-Type: application/xml

## Discussion

Change the FileVault password periodically to mitigate the security risk of deployed devices.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                             |
|----------------------------|-----------------------------|
| Device Channel             | macOS                       |
| User Channel               | \-                          |
| Requires Supervision       | \-                          |
| Allowed in User Enrollment | \-                          |
| Required Access Right      | DeviceLockAndRemovePasscode |

### Example Request and Response (Personal Recovery Key)

- Request
- Response

```

    Command

    FileVaultUnlock

        Password
        mypassword

    KeyType
    personal
    ReplyEncryptionCertificate

    MIIDKTCCAhGgAwIBAgIFAKGAf9cwDQYJKoZIhvcNAQELBQAwRTEfMB0GA1UEAwwWRmls
    ZVZhdWx0IFJlY292ZXJ5IEtleTEiMCAGA1UEDQwZR3JhaGFtcy1NYWNCb29rLVByby5s
    b2NhbDAeFw0yMDA2MTEyMzIwMjNaFw0yMTA2MTEyMzIwMjNaMEUxHzAdBgNVBAMMFkZp
    bGVWYXVsdCBSZWNvdmVyeSBLZXkxIjAgBgNVBA0MHNdyYWhhbXMtTWFjQm9vay1Qcm8u
    bG9jYWwwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDSNk47J9l7Amit4JPf
    YEj6PvqZ5nH4kPsRmoAO1FfACpzskN7gA1qui7N+O0NNjtleUI2pX8X9NvINxfPX/KTy
    eP0VXlhixvYgKMiEUkrVFBrxRtQ+7Ow80MQUAKlDBe5FVj4GyN9sAPuAu7WaJtvDAWAW
    rBSRJNqdOYpKEkgK8N9a52BmuDEBtmpaq5o5JgR2Vc+OmjcogknZi++11dKI7sDCzF3e
    jO28e9E8XNBFRO716XdyEd/VU6rE8SQmpYqrfun1pRNtiiv3dTKKn9Gl42kg7RQHjMjx
    OjmBjzWLdFrO51crcJqbT/IQ0pjWqjDcwOz9Z2gWqbtxTrrWyuJZAgMBAAGjIDAeMAsG
    A1UdDwQEAwICtDAPBgNVHRMBAf8EBTADAQEAMA0GCSqGSIb3DQEBCwUAA4IBAQCcA999
    lIN+t6u/DrTXhWlLKj8HXTmVVl8gkhxm42aZo/QsJr+gPsXF0yOWqkPpnhkrq6GVXgPx
    T7xmNv5+nDIcHX/mKRXBAUdWi/HDa3Wiytk4g9wO4xYsnBIhL5y2PHid9bSA1peKZsLL
    CX1v8vuA66trSp2fKYxW54VkLXR6xMqUcxTjp0qlfNRL6IHA6G/ogyjRkd0kt0+BwbYy
    81dDKJHVxsYOUtQlmfa8dUl20SmLwZ/bujPFetfuvWmSHrnM//J5OT4HLoGRzqXhuC/m
    XEildp3HTCm6epem3cP6Sx99aGIi08xddDzmH/5XoPmuG4uw2+ry+qbhD/UYbJbX

    RequestType
    RotateFileVaultKey

    CommandUUID
    0001_RotateFileVaultKey

```

```

    CommandUUID
    0001_RotateFileVaultKey
    RotateResult

        EncryptedNewRecoveryKey

        MIAGCSqGSIb3DQEHA6CAMIACAQAxggFqMIIBZgIBADBOMEUxHzAdBgNVBAMM
        FkZpbGVWYXVsdCBSZWNvdmVyeSBLZXkxIjAgBgNVBA0MGUdyYWhhbXMtTWFj
        Qm9vay1Qcm8ubG9jYWwCBQChgH/XMA0GDSqGSIb3DQEBAQUABIIBAFBvGbMf
        6D4hDmw3QenxL1/+3aiiMLR0Gb9hM60mnpOA9BA0o2G3QpjSRB1QBXx/Neiy
        +p3Ov1YJRdTNoECTjUSJJhxrtnj4TBykqLBlDmkuykz38ykvH85OUP17LMRh
        ThwmLVXPl9I+VZJHjFMRexjo1xiHDiIjji6o3FX2Ym0Vwt9j9+OlbN/7a6Zg
        ojVvi6DTuqxOsdr6w5ASzenWoTnahzEDJ0gijHaVV2EQOuyeHGYiBO6Y4R5x
        hpZPvw0YWY5cczRsUN+SmOuVpGNnL3wsUnDOrzbDM04u5jRkPG5v/kViTsPK
        SKLZ3UXf4kuRzUuRDSY9ScjNKmw4z7VHSU0wgAYJKoZIhvcNAQcBMBQGCCqG
        SIb3DQMHBAgwBpgbOFMR0qCABBip8ehhj0meZHHlEJYtifUFt7UIG37X/9IE
        CFaxcdPJL8tsAAAAAAAAAAAAAA==

    Status
    Acknowledged
    UDID
    99710D9B-9D05-5CC2-8BAE-590865D2753C

```

### Example Request and Response (Institutional Recovery Key)

- Request
- Response

```

    Command

    FileVaultUnlock

        Password
        mypassword

    KeyType
    institutional
    NewCertificate

    MIIDKTCCAhGgAwIBAgIFAKGAf9cwDQYJKoZIhvcNAQELBQAwRTEfMB0GA1UEAwwWRmls
    ZVZhdWx0IFJlY292ZXJ5IEtleTEiMCAGA1UEDQwZR3JhaGFtcy1NYWNCb29rLVByby5s
    b2NhbDAeFw0yMDA2MTEyMzIwMjNaFw0yMTA2MTEyMzIwMjNaMEUxHzAdBgNVBAMMFkZp
    bGVWYXVsdCBSZWNvdmVyeSBLZXkxIjAgBgNVBA0MHNdyYWhhbXMtTWFjQm9vay1Qcm8u
    bG9jYWwwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDSNk47J9l7Amit4JPf
    YEj6PvqZ5nH4kPsRmoAO1FfACpzskN7gA1qui7N+O0NNjtleUI2pX8X9NvINxfPX/KTy
    eP0VXlhixvYgKMiEUkrVFBrxRtQ+7Ow80MQUAKlDBe5FVj4GyN9sAPuAu7WaJtvDAWAW
    rBSRJNqdOYpKEkgK8N9a52BmuDEBtmpaq5o5JgR2Vc+OmjcogknZi++11dKI7sDCzF3e
    jO28e9E8XNBFRO716XdyEd/VU6rE8SQmpYqrfun1pRNtiiv3dTKKn9Gl42kg7RQHjMjx
    OjmBjzWLdFrO51crcJqbT/IQ0pjWqjDcwOz9Z2gWqbtxTrrWyuJZAgMBAAGjIDAeMAsG
    A1UdDwQEAwICtDAPBgNVHRMBAf8EBTADAQEAMA0GCSqGSIb3DQEBCwUAA4IBAQCcA999
    lIN+t6u/DrTXhWlLKj8HXTmVVl8gkhxm42aZo/QsJr+gPsXF0yOWqkPpnhkrq6GVXgPx
    T7xmNv5+nDIcHX/mKRXBAUdWi/HDa3Wiytk4g9wO4xYsnBIhL5y2PHid9bSA1peKZsLL
    CX1v8vuA66trSp2fKYxW54VkLXR6xMqUcxTjp0qlfNRL6IHA6G/ogyjRkd0kt0+BwbYy
    81dDKJHVxsYOUtQlmfa8dUl20SmLwZ/bujPFetfuvWmSHrnM//J5OT4HLoGRzqXhuC/m
    XEildp3HTCm6epem3cP6Sx99aGIi08xddDzmH/5XoPmuG4uw2+ry+qbhD/UYbJbX

    RequestType
    RotateFileVaultKey

    CommandUUID
    0001_RotateFileVaultKey

```

```

    CommandUUID
    0001_RotateFileVaultKey
    RotateResult

    Status
    Acknowledged
    UDID
    99710D9B-9D05-5CC2-8BAE-590865D2753C

```

## Topics

### Command and Response

object RotateFileVaultKeyCommand

The command to change the FileVault primary password.

object RotateFileVaultKeyResponse

A response from the device after it processes the command to change the FileVault primary password.

## See Also

### Security

Security Information

Get security-related information about a device.

List the Certificates

Get a list of installed certificates on a device.

Get the Bypass Code for Activation Lock

Get the code to bypass Activation Lock on a device.

Clear the Bypass Code for Activation Lock

Clear the Activation Lock bypass code on a device.

