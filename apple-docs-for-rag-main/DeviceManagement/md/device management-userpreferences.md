

- Device Management
-  UserPreferences 

Device Management Profile

# UserPreferences

The payload you use to configure iCloud password preferences.

macOS 10.12+Device Assignment ServicesVPP License Management

``` source
object UserPreferences
```

## Properties

`DisableUsingiCloudPassword`

`boolean`

If `true`, disables the iCloud password for local accounts.

Default: `false`

## Discussion

Specify `com.apple.preference.users` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | macOS |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            DisableUsingiCloudPassword

            PayloadIdentifier
            com.example.myuserpayload
            PayloadType
            com.apple.preferences.users
            PayloadUUID
            733ec67c-853c-45b2-9510-198e055e0723
            PayloadVersion
            1

    PayloadDisplayName
    User
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    1a5fe077-6146-44ae-82db-5cb938dddad4
    PayloadVersion
    1

```

## See Also

### Preferences

object GlobalPreferences

The payload you use to configure global preferences.

