

- Device Management
-  IdentityPreference 

Device Management Profile

# IdentityPreference

The payload you use to configure the user’s identity on the device.

macOS 10.12+Device Assignment ServicesVPP License Management

``` source
object IdentityPreference
```

## Properties

`Name`

`string`

 (Required) 

The email address (in RFC 822 format), DNS host name, or other name that uniquely identifies a service requiring this identity.

`PayloadCertificateUUID`

`string`

 (Required) 

The UUID of the certificate payload within the same profile to use for the identity credential.

## Discussion

Specify `com.apple.security.identitypreference` as the payload type.

This payload specifies an IdentityPreference item in the user’s keychain that references an identity payload included in the same profile. It can only appear in a user profile, not in a device profile.

You can include multiple IdentityPreference payloads as needed.

See also CertificatePreference for setting up certificate preferences.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | \-    |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | macOS |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            Password
            password
            PayloadContent

            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

            updated_at_xid
            23387
            PayloadIdentifier
            com.example.pkcs12payload
            PayloadType
            com.apple.security.pkcs12
            PayloadUUID
            f0100f5d-1516-4646-8cff-f68ecef626e4
            PayloadVersion
            1

            PayloadContent

            MIIDAzCCAeugAwIBAgIBATANBgkqhkiG9w0BAQsFADAvMSAwHgYD
            VQQDDBdBX1RFU1RfU01JTUVfQ0VSVElGQ0FURTELMAkGA1UEBhMC
            VVMwHhcNMTYwMjI2MTMzMjI3WhcNMTcwMjI1MTMzMjI3WjAvMSAw
            HgYDVQQDDBdBX1RFU1RfU01JTUVfQ0VSVElGQ0FURTELMAkGA1UE
            BhMCVVMwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDO
            gsJl1dKOINoO85qOl/Z8p6EXUEMxv4B5axYab1FUQp3jYa27q0Cb
            /zLiJZQGbxcfAae559gfCJPXk07roX9lKr2OlcZDJXa28/GB8Nf9
            a1xZCdeN1cGeg8gs3hvmPCWScXc1q9yE8PdFVN30w60DGx8i+ITW
            MOjySq0V3EAsmlhwxzY3w7OT9ov/1Bnnzybf+NV2m554S4zi1IY7
            yziswglf3uIGPsFGQkSZ5n6Uzlcslgw8ctp9jJD1g9Tg03LxpiQz
            6LvTjmJQvw0U1KAuBrcckVykNCYVGyxdhdZjXKylK6BKX428Ci1J
            7/NnexXyZ8k3OzH1bRZKD8roPHsbAgMBAAGjKjAoMA4GA1UdDwEB
            /wQEAwIHgDAWBgNVHSUBAf8EDDAKBggrBgEFBQcDBDANBgkqhkiG
            9w0BAQsFAAOCAQEAhVygfQK+hTxtQDOmk4ntEo3gI5HgUiiXUemA
            ZZKULTnakh5XEJ5RKoDepvgX3/sjRDwdGzpHoK7DCLhmJXsxtIGG
            drv5JitrbktWfKsWFVpnzKRWziEc6pMInzQZRyiue9ys91pbOOGo
            tF58TDUVvNN72QpnCt0MJgNCLOJFDWwdJoiJsMbBByQiDjj+pEFj
            3l72D2ms0y2ot58kZodSArW4nIOnPKbXbjsjSQz4vSOysVoNZLN2
            cdACxPf1VIEEBVRbB+2Yr8qnpC3aOJ8SvfhHfy7Qcl+R8U3ATI8w
            QO/xTI9TMNh/yMKPwsTyQKid3L2bTeTTUPC1wwyQvNwyhw==

            updated_at_xid
            23384
            PayloadIdentifier
            com.example.rootpayload
            PayloadType
            com.apple.security.root
            PayloadUUID
            c4b9ede1-2018-45b0-8e15-eb5615599027
            PayloadVersion
            1

            Name
            A_TEST_SMIME_IDENTITY_PREF
            PayloadCertificateUUID
            AF660801-04B9-4F1D-AD53-8DF76BA3F7DB
            PayloadIdentifier
            com.example.myidentitypreferencepayload
            PayloadType
            com.apple.security.identitypreference
            PayloadUUID
            e12219b3-464d-483a-84e2-069b51750c70
            PayloadVersion
            1

            Name
            A_TEST_SMIME_CERTIFICATE_PREF
            PayloadCertificateUUID
            EE61473E-9D61-4A2C-8072-FA69B2CCF4AE
            PayloadIdentifier
            com.example.mycertificatepreferencepayload
            PayloadType
            com.apple.security.certificatepreference
            PayloadUUID
            67a6046d-fd4f-4d00-9bc6-6f056bd8330f
            PayloadVersion
            1

    PayloadDescription
    Test SMIME Cert and Identity with Certificate Prefs
    PayloadScope
    User
    PayloadType
    Configuration
    PayloadUUID
    a0bc1f73-9e7d-413d-8a84-327e8e717059
    PayloadVersion
    1

```

## See Also

### Authentication

object DirectoryService

The payload you use to configure an Active Directory (AD) domain.

object ExtensibleSingleSignOn

The payload you use to configure an app extension that performs single sign-on (SSO).

object ExtensibleSingleSignOnKerberos

The payload you use to configure an app extension that performs single sign-on with the Kerberos extension.

object Identification

The payload you use to configure the names of the account user.

object SingleSignOn

The payload you use to configure single sign-on (SSO).

