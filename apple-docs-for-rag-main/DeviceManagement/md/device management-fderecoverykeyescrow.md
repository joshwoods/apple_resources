

- Device Management
-  FDERecoveryKeyEscrow 

Device Management Profile

# FDERecoveryKeyEscrow

The payload you use to configure FileVault recovery key escrow.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object FDERecoveryKeyEscrow
```

## Properties

`DeviceKey`

`string`

The string that’s included in help text if the user appears to have forgotten the password. Site admins can use this key to look up the escrowed key for the particular computer.

This key replaces the `RecordNumber` key used in the previous escrow mechanism. If the key is missing, the system uses the device serial number instead.

`EncryptCertPayloadUUID`

`string`

 (Required) 

The UUID of a payload within the same profile that contains the certificate that the system uses to encrypt the recovery key. The referenced payload must be of type `com.apple.security.pkcs1`.

`Location`

`string`

 (Required) 

The description of the location where the system escrows the recovery key. The system inserts this text into the message the user sees when it enables FileVault.

## Discussion

Specify `com.apple.security.FDERecoveryKeyEscrow` as the payload type.

FileVault Full Disk Encryption (FDE) recovery keys are, by default, sent to Apple if the user requests them. Only one payload of this type is allowed per system.

If FileVault is enabled after the system installs this payload, the system encrypts the FileVault PRK with the specified certificate, wrapped with a CMS envelope and stored at `/var/db/FileVaultPRK.dat`. The `SecurityInfo` command makes this encrypted data available to the MDM server.

Alternatively, if a site uses its own administration software, it can extract the PRK from the foregoing location at any time. Because the PRK is encrypted using the certificate provided in the profile, only the author of the profile can extract the data.

Note these cautions:

- The payload needs to exist in a system-scoped profile.

- Installing more than one payload of this type per computer results in an error.

- The previous payload (`com.apple.security.FDERecoveryRedirect`) is no longer supported. You can still install the previous payload but the system ignores it, so servers can send out the same profile to old and new clients.

- If only an old-style redirection payload is installed at the time FileVault is turned on through the Security Preferences pane, the system displays an error and doesn’t enable FileVault.

- The system doesn’t provide a warning or error if FileVault is already enabled and an old-style payload is installed. In this case, it’s assumed that the recovery key has already been escrowed with the server.

Although the system no longer supports the previous FDE Recovery payload in macOS 10.13 and later, it’s still supported in macOS 10.9 through 10.12. Designate that payload by specifying `com.apple.security.FDERecoveryRedirect` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            Password
            Password123
            PayloadContent

            MIIDHjCCAgagAwIBAgIEeRGqmzANBgkqhkiG9w0BAQsFADBAMR8w
            HQYDVQQDDBZGaWxlVmF1bHQgUmVjb3ZlcnkgS2V5MR0wGwYDVQQN
            DBRpb3MtdGFyZGlzLmFwcGxlLmNvbTAeFw0xODA2MTkyMTA2Mzla
            Fw0xOTA2MTkyMTA2MzlaMEAxHzAdBgNVBAMMFkZpbGVWYXVsdCBS
            ZWNvdmVyeSBLZXkxHTAbBgNVBA0MFGlvcy10YXJkaXMuYXBwbGUu
            Y29tMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAtOPt
            QOZ38VJMyMHWcWcs5S8D1xXVZ9OjQ7+8s7q+xNeGUZZXlHXehBHA
            iV8o7F9LvkOuJuwiWuw+9xj+ye7G4EnAtDA0p3bqZNoBIc3HIqDE
            BKTCPufqHEZfX6AH05mnYqr6fz8FbICQpx+1x6hO9f8ZSNrBJUxe
            viPCkYTvRFel9VvBS06Jijn3THFBZ9UAJjxTjU8PGQYHNRpa4pVh
            y1yIXjRwSKrmCv6NyF7vz9BQ8X4ExanGBG3P20tl5JhUTZlI+qo2
            B/ZYlQDvR+DMhrdaKtbJphdi4GNK8B87+bG7EmPCpiwLzVtkzSUK
            Y4WNbYCwUhJTjOclQsZFQKvT4QIBAQABoyAwHjALBgNVHQ8EBAMC
            ArQwDwYDVR0TAQH/BAUwAwEBADANBgkqhkiG9w0BAQsFAAOCAQEA
            rPLq0RFfAJO0Hq/Z+NLZp/EI3mBXD8a5Gq5VUepB4AYgxbmtS5Dr
            XJMlzi1ctYGj3+QN+9XbgNv/p3cphHvSBmvFmjL8gJ6AuqNG9/hV
            TYEsoS5i9pGIlWozTziS+EPbdHt76g4xOOPoQ3SDur+qpc3Hfi1A
            imCaRB2Ga/eIITDqQUi1Sfgz0r0Md0jIEpXnW8RSvAQm9tlt35os
            onzTvHiKjXkOxBrXGg84YSK9/MsvwcPUM/XZ9HmZMTVYnPRacZlX
            9m4yKJligP7vmSjpbQ6u5zngsilhLUezX9stOyduAKLxk354yW85
            CQEgrRbwQQzGSWlf8KV0sbubwz4H8w==

            PayloadIdentifier
            com.example.mypkcs1payload
            PayloadType
            com.apple.security.pkcs1
            PayloadUUID
            5ddd0439-620a-4939-8bbc-838ae490b12f
            PayloadVersion
            1

            Defer

            DeferDontAskAtUserLogout

            DeferForceAtUserLoginMaxBypassAttempts
            -1
            Enable
            On
            PayloadCertificateUUID
            5ddd0439-620a-4939-8bbc-838ae490b12f
            ShowRecoveryKey

            UseKeychain

            UseRecoveryKey

            UserEntersMissingInfo

            PayloadIdentifier
            com.example.myfv2payload
            PayloadType
            com.apple.MCX.FileVault2
            PayloadUUID
            8d5d8dfb-688a-436d-b827-b81e550702b3
            PayloadVersion
            1

            EncryptCertPayloadUUID
            5ddd0439-620a-4939-8bbc-838ae490b12f
            Location
            Your Information is now escrowed
            PayloadIdentifier
            com.example.myfderecoverykeyescrowpayload
            PayloadType
            com.apple.security.FDERecoveryKeyEscrow
            PayloadUUID
            202ffa93-e1ae-43b5-b9de-e656ac0c2045
            PayloadVersion
            1

    PayloadDisplayName
    FDE Recovery Key Escrow
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    bf625ece-5e99-489b-b197-6f1d7c52a601
    PayloadVersion
    1

```

## See Also

### Full Disk Encryption

object FDEFileVault

The payload you use to configure FileVault.

object FDEFileVaultOptions

The payload you use to configure FileVault options.

