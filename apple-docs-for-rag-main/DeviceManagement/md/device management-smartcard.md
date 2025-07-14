

- Device Management
-  SmartCard 

Device Management Profile

# SmartCard

The payload you use to configure a smart card.

macOS 10.12.4+Device Assignment ServicesVPP License Management

``` source
object SmartCard
```

## Properties

`allowSmartCard`

`boolean`

If `false`, the system disables the SmartCard for logins, authorizations, and screen saver unlocking. It is still allowed for other functions, such as signing emails and accessing the web. A restart is required for a setting change to take effect.

Default: `true`

`checkCertificateTrust`

`integer`

Configures the certificate trust check and has one of the following possible values:

- `0`: Turns off certificate trust check.

- `1`: Turns on certificate trust check. A standard validity check is performed but doesn’t include additional revocation checks.

- `2`: Turns on certificate trust check. A soft revocation check is also performed. Until the certificate is explicitly rejected by CRL/OCSP, it’s considered valid. This setting means that unavailable or unreachable CRL/OCSP allow this check to succeed.

- `3`: Turns on certificate trust check. A hard revocation check is also performed. Unless CRL/OCSP explicitly says “This certificate is OK,” it’s considered invalid. This option is the most secure.

Default: `0`

Possible Values: `0, 1, 2, 3`

`enforceSmartCard`

`boolean`

If `true`, a user can only log in or authenticate with a SmartCard. Available in macOS 10.13.2 and later.

Default: `false`

`oneCardPerUser`

`boolean`

If `true`, a user can pair with only one SmartCard, although existing pairings are allowed if already set up.

Default: `false`

`tokenRemovalAction`

`integer`

If `1`, the system enables the screen saver when the SmartCard is removed. Available in macOS 10.13.4 and later.

Default: `0`

Possible Values: `0, 1`

`UserPairing`

`boolean`

If `false`, users don’t get the pairing dialog, although existing pairings still work.

Default: `true`

## Discussion

Specify `com.apple.security.smartcard` as the payload type.

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

            UserPairing

            allowSmartCard

            checkCertificateTrust

            oneCardPerUser

            tokenRemovalAction
            1
            enforceSmartCard

            PayloadIdentifier
            com.example.mysmartcardpayload
            PayloadType
            com.apple.security.smartcard
            PayloadUUID
            88f7336c-d9f6-44d1-b486-11e4080e2223
            PayloadVersion
            1

    PayloadDisplayName
    SmartCard
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    85091214-a32f-4131-8b03-0045e5d81c42
    PayloadVersion
    1

```

## See Also

### Security

object Passcode

The payload you use to configure a passcode policy.

object SecurityPreferences

The payload you use to configure security preferences.

