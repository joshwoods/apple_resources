

- Device Management
-  GlobalPreferences 

Device Management Profile

# GlobalPreferences

The payload you use to configure global preferences.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object GlobalPreferences
```

## Properties

`com.apple.autologout.AutoLogOutDelay`

`number`

The `autologout` delay, in seconds. A value of `0` means `autologout` is off. In some cases, this delay may be restricted to values between 5 minutes and 24 hours.

`MultipleSessionEnabled`

`boolean`

If `false`, disables fast user switching.

Default: `true`

## Discussion

Specify `.GlobalPreferences` as the payload type.

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

            MultipleSessionEnabled

            com.example.autologout.AutoLogOutDelay
            1800
            LULookupDisabled

            PayloadIdentifier
            com.example.myglobalpayload
            PayloadType
            .GlobalPreferences
            PayloadUUID
            b5033127-c0ef-4055-8fc5-7db5a8216bc8
            PayloadVersion
            1

    PayloadDisplayName
    Global Preferences
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    52e0e1b6-067f-407a-a36c-7e7b917b2982
    PayloadVersion
    1

```

## See Also

### Preferences

object UserPreferences

The payload you use to configure iCloud password preferences.

