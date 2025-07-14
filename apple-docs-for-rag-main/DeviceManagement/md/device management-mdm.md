

- Device Management
-  MDM 

Device Management Profile

# MDM

The payload you use to configure mobile device management (MDM) settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object MDM
```

## Properties

`AccessRights`

`integer`

Logical OR of the following bit flags:

`1`  
Allow inspection of installed configuration profiles.

`AssignedManagedAppleID`

`string`

`CheckInURL`

`string`

`CheckInURLPinningCertificateUUIDs`

`[string]`

`CheckOutWhenRemoved`

`boolean`

Default: `false`

`EnrollmentMode`

`string`

Possible Values: `BYOD, ADDE`

`IdentityCertificateUUID`

`string`

 (Required) 

`ManagedAppleID`

`string`

Deprecated 

`PinningRevocationCheckRequired`

`boolean`

Default: `false`

`PromptUserToAllowBootstrapTokenForAuthentication`

`boolean`

Default: `false`

`RequiredAppIDForMDM`

`integer`

`ServerCapabilities`

`[string]`

Possible Values: `com.apple.mdm.per-user-connections, com.apple.mdm.bootstraptoken, com.apple.mdm.token`

`ServerURL`

`string`

 (Required) 

`ServerURLPinningCertificateUUIDs`

`[string]`

`SignMessage`

`boolean`

Default: `false`

`Topic`

`string`

 (Required) 

`UseDevelopmentAPNS`

`boolean`

Default: `false`

## Mentioned in 

Managing MDM Devices and Users in macOS

## Overview

`2`  
Allow installation and removal of configuration profiles.

`4`  
Allow device lock and passcode removal.

`8`  
Allow device erase.

`16`  
Allow query of device information (device capacity, serial number).

`32`  
Allow query of network information (phone/SIM numbers, MAC addresses).

`64`  
Allow inspection of installed provisioning profiles.

`128`  
Allow installation and removal of provisioning profiles.

`256`  
Allow inspection of installed applications.

`512`  
Allow restriction-related queries.

`1024`  
Allow security-related queries.

`2048`  
Allow manipulation of settings.

`4096`  
Allow app management.

Don’t set to `0`. Specify `1` if you specify `2`. Specify `64` if you specify `128`. Ignored if you set a value for `ManagedAppleID`.

- AssignedManagedAppleID: The Managed Apple ID pre-assigned to the authenticated user. The system only uses this value with account-driven enrollment. When updating the payload, the value of this key must not change. Any change is an error, and the update rejected. Available in iOS 15 and later.

- CheckInURL: The URL that the device should use to check in during installation. The URL must begin with the `https://` URL scheme and may contain a port number (`:1234`, for example). If not set, the system uses `ServerURL`.

- CheckInURLPinningCertificateUUIDs: An array of strings, each containing the payload UUID of a certificate to use when evaluating trust to the `.../checkin/` URLs of MDM servers.

- CheckOutWhenRemoved: If `true`, the device attempts to send a CheckOut message to the `CheckInURL` when the profile is removed.

- EnrollmentMode: The enrollment mode the server indicates to use when enrolling. Required for BYOD enrollments and for the profile-based user enrollment flow. Don’t set for the account-based user enrollment flow. Available in iOS 15 and later.

- IdentityCertificateUUID: The UUID of the certificate payload for the device’s identity. It may also point to a SCEP payload.

- ManagedAppleID: The Managed Apple ID of the user. Required for the profile-based user enrollment flow. Don’t set for the account-based user enrollment flow. Available in iOS 13.1 and later, and macOS 10.15 and later.

- PinningRevocationCheckRequired: If `true`, the system fails the connection attempt unless it obtains a verified positive response during certificate revocation checks.

  If `false`, the system performs revocation checks on a best-attempt basis, where failure to reach the server isn’t considered fatal.

- PromptUserToAllowBootstrapTokenForAuthentication: If `true`, the system warns the user that they need to reboot into RecoveryOS and allow the MDM to use the Bootstrap Token for authentication for certain sensitive operations such as enabling kernel extensions or installing some types of software updates. If the MDM doesn’t need to perform these operations, it can leave this key set to `false`, and the user isn’t notified.

  The SettingsCommand.Command.Settings.MDMOptions.MDMOptions command overrides this default value.

  This setting only applies to devices that have `BootstrapTokenRequiredForSoftwareUpdate` or `BootstrapTokenRequiredForKernelExtensionApproval` set to `true` in their SecurityInfoResponse.SecurityInfo.

  DEP-enrolled devices are automatically allowed to use the Bootstrap Token for authentication.

  Available in macOS 11 and later.

- RequiredAppIDForMDM: This property specifies an iTunes Store ID for an app the system can install with the InstallApplicationCommand, without any approval from the user. The MDM vendor or managing organization generally provides this app, which enhances the management experience for the user. The device shows the user details about this app in the account-driven enrollment process prior to installing the MDM profile. Use this property with account-driven MDM enrollments that normally require user approval for app installs through MDM.

  Only account-driven user enrollments support this property and other enrollment types ignore it.

  Available in iOS 15.1 and later.

- ServerCapabilities: A unique array of strings indicating server capabilities. If the server manages macOS devices or a Shared iPad, this field is mandatory and must contain the value `com.apple.mdm.per-user-connections`, which indicates that the server supports both device and user connections.

  Starting with macOS 11, it’s also recommended that macOS device enrollment profiles contain the value `com.apple.mdm.bootstraptoken` to ensure the Bootstrap Token is created and escrowed with the MDM server at enrollment time.

- ServerURL: The URL that the device contacts to retrieve device management instructions. The URL must begin with the `https://` URL scheme, and may contain a port number (`:1234`, for example).

- ServerURLPinningCertificateUUIDs: An array of strings, each containing the UUID of a certificate to use when evaluating trust to the `.../connect/` URLs of MDM servers.

- SignMessage: If `true`, each message coming from the device carries the additional `Mdm-Signature` HTTP header.

- Topic: The topic that MDM listens to for push notifications. The certificate that the server uses to send push notifications must have the same topic in its subject. The topic must begin with the `com.apple.mgmt.` prefix.

- UseDevelopmentAPNS: If `true`, the device uses the development APNS servers. Otherwise, the device uses the production servers.

  Set to `false` if your Apple Push Notification Service certificate was issued by the Apple Push Certificate Portal (`https://identity.apple.com/pushcert`). That portal only issues certificates for the production push environment.

## Discussion

Also define the following four standard payload values in your MDM payload:

`PayloadIdentifier`  
The reverse-DNS style identifier that identifies the profile; for example, `com.example.myprofile`. The system uses this value to determine whether to replace an existing profile or add a new one.

`PayloadUUID`  
A globally unique identifier for the profile. In macOS, you can use `uuidgen` to generate this value.

`PayloadType`  
The payload type. Set to `com.apple.mdm` to designate that this payload is an MDM payload.

`PayloadVersion`  
The version number of the profile format, which describes the version of the configuration profile as a whole, not of the individual profiles within it. Set this value to `1`.

Note

MDM reserves profile payload dictionary keys with the *Payload* prefix. Don’t treat them as managed preferences.

### Profile Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | \-                                     |
| Allow Manual Install       | iOS, macOS, tvOS                       |
| Requires Supervision       | watchOS                                |
| Requires User Approved MDM | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Allow Multiple Payloads    | \-                                     |

### Profile Example

```

    PayloadContent

            PayloadContent

            LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUZlRENDQTJB
            Q0NRQzFsWFV5WnJPbERqQU5CZ2txaGtpRzl3MEJBUXNGQURCK01R
            c3dDUVlEVlFRR0V3SlYKVXpFVE1CRUdBMVVFQ0F3S1EyRnNhV1p2
            Y201cFlURVNNQkFHQTFVRUJ3d0pRM1Z3WlhKMGFXNXZNUk13RVFZ
            RApWUVFLREFwQmNIQnNaU0JKYm1NdU1Sb3dHQVlEVlFRTERCRkVa
            WFpwWTJVZ1RXRnVZV2RsYldWdWRERVZNQk1HCkExVUVBd3dNVFVN
            Z1VtOXZkQ0JEWlhKME1CNFhEVEU1TURVd01UQTNNVFF6TVZvWERU
            STVNRFF5T0RBM01UUXoKTVZvd2ZqRUxNQWtHQTFVRUJoTUNWVk14
            RXpBUkJnTlZCQWdNQ2tOaGJHbG1iM0p1YVdFeEVqQVFCZ05WQkFj
            TQpDVU4xY0dWeWRHbHViekVUTUJFR0ExVUVDZ3dLUVhCd2JHVWdT
            VzVqTGpFYU1CZ0dBMVVFQ3d3UlJHVjJhV05sCklFMWhibUZuWlcx
            bGJuUXhGVEFUQmdOVkJBTU1ERTFESUZKdmIzUWdRMlZ5ZERDQ0Fp
            SXdEUVlKS29aSWh2Y04KQVFFQkJRQURnZ0lQQURDQ0Fnb0NnZ0lC
            QUpZVUFISWErRHI1Q0JzeEQ5NjJTRTc1WG50UzNmTEYyRGJIdHFT
            YwpwdXpsRVhEeC8yaXNVWHVKVkhYdlNkWkx3YmpFRFJKMTF5WlNv
            SzFTMTJVOFVUS1VsK2JHUS9HbjcxVkJnblY2CmFxYmRWVzRFOGxJ
            bU1rN2paRE1IMW14a3cxOWZHdEREaEVOMTA1R3g3K2RVbkpzMTdz
            NHAramJIUThwbzNIY2sKNG5VejgyVTZKUmJXdU5SZFNxNWIvaDNT
            VzlBM2laMXRPRHlNbExOK1ZyaHREYkxhRS9URlk1eFovdjRiUmZ2
            RQpGSjYvVVQ2bGc3RVorcjBYdnljV0tvMnZUL2ZPdUVHbU5CczFy
            YmNPZ3dpQlZEUjdXRG5Pb3RUVkHtMUxydFZFCmFtVlljUHdxSjlu
            Y01hSk14Y01JNHZDazR4eFBwNy9jeEJzcGQwK2diR1lYSVlkYnI5
            YlM2Q1RhMHkzTmIxeCsKdnJZN1RTWFBHSFRNQzAvYXBQQ21CRjBy
            RFdzNm1ZcytFKzRQaENLaDUyeFRROHp5WjVRNk5yOVhqUVJKajl2
            YgpKa2pMMTY1NnJwVFBFV21CUzJxQ1ZqTUxpbFA4MGE1MDVkd0kx
            YzZwa1NrUDczMGtIaExtQ1R4ZkJwb1Jid1p5CjFrQk1qM2xhWkE5
            Y21UUlFiT1pQMkYzNVVudmw1LzFuNG5Wd0N4R1Mzc2U1NWxudzh3
            SzUvRmtBYXptS1dDdzAKTnZjRUc5T0FtQUIrNWpaVVdNZXdoenFy
            TWdMUDFQbm1qR0twemN0dG8vTmxQZE91QVhnZ1A0ZjlPaVkyNlV4
            UwpHcW55R2hXamlIbTZIeXkvMWNuNXRYZVNMcVZISzZoaXJINk1o
            eks4K0R5Rkg2N0R3dmIyTnRKUkhadUhTb0FXClRwS2ZBZ01CQUFF
            d0RRWUpLb1pJaHZjTkFSSUxCUUFEZ2dJQkFHVWl4VDEwaW5KcVVq
            b0NtTWpHNlJwL1hGRUgKZzZoQml6OFUveVJWUEhvMG9RNFREdnIw
            WDBFOXk3Lyt3YXc5clpIRTdqd1VOendtWXZFeWwwMzZCcFQyVVZB
            aQpvWDAyMDZqcmVXSk9nTVYxbFlBVWhYZTY1eml2ak9WRE9rVFFX
            aUZKb3pjbXYwdXZabmsrRWl4eFByUEJYOThOClhRNEF5VWt5S25n
            WTVHSnlPbW5iK3ZnUlFCM25yTXpJbXIyekxNUlp2b21DT1pEV0FK
            ZGF3UlNZTXBFOGZreVAKZnY3QzVWOXdLVllxVFJNd1FEbk1YL1g5
            eUFUTXV0QWV0MTV3N2taN3JYenc4ZFxjZFBwMlBSQkJIem1kWWF3
            egpmbFdWT2dBKzdHSTcwVkVtNER6UkxCVmJjaUcyZU1mVEtYemZX
            eGcrbHhQaWxacy82T2Y1aG9jdVRWeVhEeHJnCkUwRDZLbFVSK2k0
            N3ovZDRTaWsrSVdJRkx3Y21XOEhFelEyVzlTakFwSDRTaGhEKzBz
            UXQ2bzZMNjA0cjBqTzEKbUhYbkhxSmNGRmVaYjlONzJrMElNZTJv
            MForaXd1YmJYamZQZzlMV1EzamVJOVJPZkJzWlA1ZkE1MkxiRlB5
            UgpiSkxOODl4cm5DeEt2TzVsUHp2WHpwYXlrRUNWRG1Oa0lZMlRO
            WG4yUnVmQVdDYXpFVWlLd2lPQ1JLZjJSTHBPCmZUb25IYVdIZi9B
            NzBqWTJXb1JGQ3laV1BnQ3U2QW1kMFNNK3p2cm1NQi9SLzZBYlQv
            WDFjckFQR1ArNkVzU0YKeHBkRHJqZUdLYWlYM3l0UmVBSnFFMEFQ
            YWt4OENXR2haMkVVOUlnY3loNTE2bGY4OXlUcTBEbGlCUjNDWVJl
            bgpsMGJhMSt6M1J6VlZhRWgvCi0tLS0tRU5EIENFUlRJRklDQVRF
            LS0tLS0K

            PayloadIdentifier
            com.example.mypempayload
            PayloadType
            com.apple.security.pem
            PayloadUUID
            0dfe81fe-e8f6-45c0-9860-2c893fe30114
            PayloadVersion
            1

            PayloadContent

                URL
                https://mdm.example.com:2002/scep
                Key Type
                RSA
                Key Usage
                5
                Keysize
                2048
                Subject

                            O
                            Example, Inc.

                            CN
                            Device Certificate

                Challenge
                MDMEnrollment

            PayloadIdentifier
            com.example.mysceppayload
            PayloadType
            com.apple.security.scep
            PayloadUUID
            47492623-e4e7-4a64-ba63-2f31d2ca1a5f
            PayloadVersion
            1

            IdentityCertificateUUID
            47492623-e4e7-4a64-ba63-2f31d2ca1a5f
            ServerURL
            https://mdm.example.com:2001/mdm
            Topic
            com.apple.mgmt.External.c809ab17-1cbd-48f2-8dc7-e952131df20c
            AccessRights
            8191
            ServerCapabilities

                com.apple.mdm.per-user-connections
                com.apple.mdm.bootstraptoken

            CheckInURL
            https://mdm.example.com:2001/checkin
            CheckOutWhenRemoved

            PromptUserToAllowBootstrapTokenForAuthentication

            PayloadIdentifier
            com.example.mymdmpayload
            PayloadType
            com.apple.mdm
            PayloadUUID
            0ae4af50-590a-4478-b540-aa0a21da23f1
            PayloadVersion
            1

    PayloadDisplayName
    MDM
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    1f4ef23b-ab01-45b9-879c-7a036e47b083
    PayloadVersion
    1

```

## See Also

### Managed Devices

object EducationConfiguration

The payload you use to configure the users, groups, and departments within an educational organization.

object LightsOutManagementLOM

The payload you use to configure lights-out management (LOM) settings.

object ManagedPreferences

The payload you use to configure managed preferences.

object ProfileRemovalPassword

The payload you use to configure profile removal.

