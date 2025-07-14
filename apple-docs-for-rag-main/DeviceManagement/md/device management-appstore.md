

- Device Management
-  AppStore 

Device Management Profile

# AppStore

The payload you use to configure macOS App Store restrictions.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object AppStore
```

## Properties

`DisableSoftwareUpdateNotifications`

`boolean`

If `true`, the system disables software update notifications. Available in macOS 10.10 and later.

Default: `false`

`restrict-store-disable-app-adoption`

`boolean`

If `true`, the system disables app adoption by users. Available in macOS 10.10 and later.

Default: `false`

`restrict-store-require-admin-to-install`

`boolean`

Deprecated 

If `true`, the system restricts app installations to admin users only. Deprecated in macOS 10.14. Use the `com.apple.SoftwareUpdate` payload key `restrict-software-update-require-admin-to-install` instead.

Default: `false`

`restrict-store-softwareupdate-only`

`boolean`

If `true`, the system prevents App Store from launching. Available in macOS 10.14 and later. Restricts installations to software updates only in macOS 10.10 through 10.13.

Default: `false`

## Discussion

Specify `com.apple.appstore` as the payload type.

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

            DisableSoftwareUpdateNotifications

            restrict-store-disable-app-adoption

            restrict-store-softwareupdate-only

            PayloadIdentifier
            com.example.myappstorepayload
            PayloadType
            com.apple.appstore
            PayloadUUID
            44561b1a-c66c-42b8-80cd-c30a29766e34
            PayloadVersion
            1

    PayloadDisplayName
    App Store
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    61c30df8-92e8-4fc5-8623-8cfc294452ce
    PayloadVersion
    1

```

