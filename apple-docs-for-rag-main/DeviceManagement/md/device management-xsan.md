

- Device Management
-  Xsan 

Device Management Profile

# Xsan

The payload you use to configure an Xsan client system.

macOS 10.10+Device Assignment ServicesVPP License Management

``` source
object Xsan
```

## Properties

`fsnameservers`

`[string]`

An array of storage area network (SAN) File System Name Server coordinators. The list should contain the same addresses in the same order as the metadata controller (MDC) `/Library/Preferences/Xsan/fsnameservers` file. Xsan SAN clients automatically receive updates to the `fsnameservers` list from the SAN configuration servers whenever this list changes. StorNext administrators should update their profile whenever the `fsnameservers` list changes.

This key is required for StorNext SANs.

`sanAuthMethod`

`string`

The authentication method for the SAN. This key is required for all Xsan SANs. It’s optional for StorNext SANs but should be set if the StorNext SAN uses an `auth_secret` file.

Only one value is accepted: `auth_secret`

Value: `auth_secret`

`sanConfigURLs`

`[string]`

An array of LDAP URLs where Xsan systems can obtain SAN configuration updates. This key is required for all Xsan SANs. There should be one entry for each Xsan MDC.

Example URL: `ldaps://mdc1.example.com:389`.

`sanName`

`string`

 (Required) 

The name of the SAN. This key is required for all Xsan SANs. The name must exactly match the name of the SAN defined in the metadata server.

`sharedSecret`

`string`

 (Required) 

The shared secret used for Xsan network authentication. This key is required when the `sanAuthMethod` key is present. The value should equal the content of the MDC’s `/Library/Preferences/Xsan/.auth_secret` file.

## Discussion

Specify `com.apple.xsan` as the payload type.

For more information, see https://support.apple.com/en-us/HT205333.

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

            fsnameservers

                san.example.com

            sanAuthMethod
            auth_secret
            sanName
            user_xsan
            sharedSecret
            shared_secret
            PayloadIdentifier
            com.example.myxsanpayload
            PayloadType
            com.apple.xsan
            PayloadUUID
            015b6f29-6a6a-4e23-9305-a4182838516d
            PayloadVersion
            1

    PayloadDisplayName
    Xsan
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    e93b1eca-d07c-4383-8b4f-ca9db76f4aa8
    PayloadVersion
    1

```

## See Also

### Xsan

object XsanPreferences

The payload you use to configure the Xsan preferences that define the volumes that automatically mount at startup.

