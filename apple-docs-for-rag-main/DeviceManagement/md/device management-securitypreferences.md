

- Device Management
-  SecurityPreferences 

Device Management Profile

# SecurityPreferences

The payload you use to configure security preferences.

macOS 10.10+Device Assignment ServicesVPP License Management

``` source
object SecurityPreferences
```

## Properties

`dontAllowFireWallUI`

`boolean`

If `true`, disables user changes to the firewall settings.

Default: `false`

`dontAllowLockMessageUI`

`boolean`

If `true`, disables user changes to the lock message.

Default: `false`

`dontAllowPasswordResetUI`

`boolean`

If `true`, disables user changes to the password.

Default: `false`

## Discussion

Specify `com.apple.preference.security` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            dontAllowFireWallUI

            PayloadIdentifier
            com.example.mysecuritypreferencespayload
            PayloadType
            com.apple.preference.security
            PayloadUUID
            d99bb019-a61d-447f-8fed-8f223cc56be3
            PayloadVersion
            1

    PayloadDisplayName
    Security Preferences
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    b44b6a04-6527-4333-87e5-46422e8a5844
    PayloadVersion
    1

```

## See Also

### Security

object Passcode

The payload you use to configure a passcode policy.

object SmartCard

The payload you use to configure a smart card.

